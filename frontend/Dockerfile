# 1. Use the official Node image
FROM node:20-alpine

# 2. Set the working directory
WORKDIR /app

# 3. Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# 4. Copy the rest of your application code
COPY . .

# 5. Expose your app's port (change if your app uses a different port)
EXPOSE 5173

# 6. Run the npm start command
CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0"]