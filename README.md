

# PHÁT TRIỂN ỨNG DỤNG GHI CHÉP VÀ LẬP KẾ HOẠCH DOLS NOTES & PLANS MANAGEMENT APP

![image](https://i.ibb.co/HF5XXy0/cb9164b93325ea7bb334.jpg)

Bạn có thể xem readme dưới dạng website bằng link dưới đây
[xem-online](https://github.com/dinhoangduy/showreadme/blob/main/README.md).



## HƯỚNG TRIỂN KHAI DỰ ÁN

Trong thư mục này gồm có: file readme(file đang đọc), file tài liệu(docs), folder source.

Để triển khai dự án vui lòng thực hiện theo các bước dưới đây:

### TRIỂN KHAI CHO SERVER
Chọn folder server
- Node version >=12 & < 17
- Nếu đã có file database. Hãy restore database. Config lại DB_NAME, DB_PORT, DB_HOST, DB_PASS, DB_USER
Sau đó chạy source ở local bằng 
  npm install
  npm run dev

### TRIỂN KHAI CHO CLIENT

Truy cập vào source/client

Lưu ý: nodejs version 16.17.1

Đầu tiên dependencies cho dự án

    yarn hoặc npm install

Sau đó thay đổi link server ở file api/axiosClient.js dòng 4

    const baseUrl = [link-server]

Khởi chạy dự án
    
    yarn start


### TRIỂN KHAI CHO ADMIN

Truy cập vào source/admin

Lưu ý: nodejs version 16.16.0

Đầu tiên dependencies cho dự án

    yarn hoặc npm install

Sau đó thay đổi link server ở file api/axiosClient.js dòng 5

    const baseUrl = [link-server]

Khởi chạy dự án
    
    yarn run dev
    
### TRIỂN KHAI FIREBASE CHO DỰ ÁN

Truy cập: https://firebase.google.com/  ==> Get started ==> Tạo project web trên firebase 

Sử dụng Storage và Authentication - Sign-in providers with google của FIRABASE

Vào Authentication -> Setting -> Authorized domains: cấp phép sử dụng

--- Kết nối firabase cho dự án
Truy cập /fỉrebase.js đỗi lại thông tin trong firebaseConfig - từ dòng 5 (lưu ý không đỗi apiKey trong file này).

Truy cập vào các biến .env.* đỗi lại biến VITE_APP_FIRABASE_KEY bằng firabase key.



