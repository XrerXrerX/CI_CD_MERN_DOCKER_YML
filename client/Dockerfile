FROM node:13-alpine

# Buat direktori /home/app untuk proyek
RUN mkdir -p /home/app

# Set working directory ke dalam direktori /home/app
WORKDIR /home/app

# Copy file package.json dan package-lock.json ke direktori /home/app
COPY . /home/app

# Install dependensi menggunakan npm
RUN npm install

CMD ["sh", "-c", "cd /home/app && npm run start"]
