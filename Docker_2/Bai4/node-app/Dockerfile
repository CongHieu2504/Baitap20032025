# Sử dụng image Node.js chính thức
FROM node:16

# Tạo thư mục làm việc trong container
WORKDIR /usr/src/app

# Sao chép tệp package.json và package-lock.json vào container
COPY package*.json ./

# Cài đặt các package Node.js
RUN npm install

# Sao chép toàn bộ mã nguồn vào container
COPY . .

# Mở cổng 3000
EXPOSE 3000

# Chạy ứng dụng Node.js
CMD ["node", "app.js"]
