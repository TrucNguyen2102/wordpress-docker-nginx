Đây là project môn chuyên đề CNPM của thầy Lê Hà Thanh.
Link: Tài liệu triển khai: https://drive.google.com/drive/folders/1Rb2Wff80fpQBTgVdlVikJwEs5b7LjoN3?usp=sharing
<!-- ttttt -->
Các bước thực hiện:
- Clone project về.
- Khi clone về, cần xác định file project được đặt ở đâu?
- Mở file project bằng visual studio code.
- Xác định đường dẫn dẫn đến file docker-compose.yml.
    + Trong file này bạn có thể config port của service wordpress nếu bạn muốn.
    + port của mysql mặc định là 3306, nếu bạn bị báo lỗi thì đừng quá lo lắng. Do có 1 service nào đó sử dụng port này, chẳng hạn như MySQL trên máy của bạn, chỉ cần stop MySQL trên máy bạn là có thể cài đặt bình thường.
- Chạy project: yêu cầu đã cài đặt Docker Desktop trên máy
    + Mở terminal trong visual studio code và nhập lệnh sau: docker compose up -d
    + Chờ quá trình cài đặt (có thể mất vài phút do lần đầu cài đặt)
    + Nếu bạn có sự thay đổi nào trong file docker-compose.yml, bạn nhập lệnh sau để xóa quá trình cài đặt trước: docker compose down và nhập lệnh: docker compose up -d để cập nhật lại những thay đổi.
- config file nginx.conf: bạn cần config file này phù hợp để có thể build được tốt nhất.
- Khi build thành công, bạn vào docker sẽ thấy xuất hiện các service.
