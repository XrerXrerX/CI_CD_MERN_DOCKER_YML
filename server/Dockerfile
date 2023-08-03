FROM node:18-alpine

ENV MONGO_URL=mongodb://admin:admin@mongodb:27017 
ENV PORT=3001 
ENV JWT_SECRET=qq123456

# Buat direktori /home/app untuk proyek
RUN mkdir -p /home/app

# Set working directory ke dalam direktori /home/app
WORKDIR /home/app

# Copy file package.json dan package-lock.json ke direktori /home/app
COPY . /home/app

# Install dependensi menggunakan npm
RUN npm install

CMD ["sh", "-c", "cd /home/app && npm run start"]