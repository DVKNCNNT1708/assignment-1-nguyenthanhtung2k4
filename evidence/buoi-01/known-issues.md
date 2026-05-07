# Known Issues · Buổi 1

Ghi lại lỗi chưa xử lý được hoặc đã xử lý xong.

| STT | Lỗi gặp phải | Lệnh gây lỗi | Cách đã thử | Trạng thái |
|---:|---|---|---|---|
| 1 | Docker daemon/pipe chưa truy cập được; Docker CLI đã có version nhưng các lệnh cần daemon bị timeout hoặc báo `Access is denied` với `\\.\pipe\docker_engine`. | `docker info`, `docker image ls`, `docker run --rm hello-world`, `.\scripts\collect_session01_evidence.ps1` | Đã tìm thấy Docker CLI tại `C:\Program Files\Docker\Docker\resources\bin`, đã thêm PATH tạm thời, đã xác nhận Docker Compose CLI có version. Kiểm tra thấy service `com.docker.service` đang `Stopped`. | Chưa xử lý xong. Cần mở Docker Desktop, nếu vẫn lỗi thì chạy PowerShell bằng Run as administrator rồi chạy lại `.\scripts\collect_session01_evidence.ps1`. |
| 2 | `conda env list` gặp lỗi permission/plugin trong sandbox, nhưng môi trường Python chính vẫn chạy được. | `conda env list` | Kiểm tra trực tiếp bằng `C:\Users\tungb\anaconda3\envs\api-platform\python.exe --version`. Kết quả: Python 3.11.15. | Đã xử lý bằng cách xác nhận trực tiếp Python trong env `api-platform`; không chặn bài nộp. |
