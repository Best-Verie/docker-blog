FROM node:17-alpine
RUN npm add -g pnpm
WORKDIR /app
ENV PATH /app/node_modules/.bin:$PATH
COPY ./package.json /app/
RUN pnpm install --force
COPY . /app
RUN pnpm build
EXPOSE 3000
CMD ["pnpm","preview"]