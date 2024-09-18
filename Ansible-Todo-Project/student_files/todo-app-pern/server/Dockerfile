# Node.js image'ini kullan
FROM node:18

# Uygulama dosyalarının kopyalanacağı dizin
WORKDIR /usr/src/app

# package.json ve package-lock.json dosyalarını kopyala
COPY package*.json ./

# Bağımlılıkları yükle
RUN npm install

# Uygulama dosyalarını kopyala
COPY . .

# Node.js uygulamasının çalışacağı portu aç
EXPOSE 5000

# Uygulamayı başlat
CMD ["npm", "start"]

