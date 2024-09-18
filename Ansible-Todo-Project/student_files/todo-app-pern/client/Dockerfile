# Node.js image'ini kullan
FROM node:18

# Uygulama dizinini oluştur
WORKDIR /usr/src/app

# package.json ve package-lock.json dosyalarını kopyala
COPY package*.json ./

# React bağımlılıklarını yükle
RUN npm install

# Uygulama dosyalarını kopyala
COPY . .

# React uygulaması için build yap
RUN npm run build

# React servisini başlat
EXPOSE 3000

# React uygulamasını çalıştır
CMD ["npm", "start"]
