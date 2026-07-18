FROM node:22-alpine

WORKDIR /app

# Copy backend package files
COPY backend/package*.json ./

# Copy shared folder to parent directory (so ../shared works)
COPY shared ../shared

# Install dependencies
RUN npm install

# Copy backend source code
COPY backend .

EXPOSE 3000

CMD ["npm", "start"]

