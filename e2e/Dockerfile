FROM mcr.microsoft.com/playwright:v1.52.0-noble

WORKDIR /e2e

COPY package.json package-lock.json* ./

RUN npm install

COPY tests ./tests
COPY .env .
COPY playwright.config.ts .

RUN mkdir /e2e/test-results
VOLUME /e2e/test-results

CMD ["npx", "playwright", "test"]