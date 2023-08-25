FROM node:16-alpine

WORKDIR /app
RUN npm install --global pnpm
COPY package.json .
RUN pnpm install --prod
COPY . .

CMD ["pnpm", "run", "dev"]
