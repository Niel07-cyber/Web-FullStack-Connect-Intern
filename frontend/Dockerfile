# frontend/Dockerfile
FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
# Remove the production build step
# RUN npm run build
EXPOSE 3000
# Use development server instead of production
CMD ["npm", "run", "dev"]