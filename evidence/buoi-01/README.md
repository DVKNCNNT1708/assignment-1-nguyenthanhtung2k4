# Minh chứng Buổi 1

Thư mục này dùng để nộp minh chứng thiết lập môi trường lab và xác định service boundary cho đề tài A4.

## Thông tin sinh viên

- Họ tên: Nguyễn Thanh Tùng
- Mã sinh viên: 1771020729
- Nhóm: 3 Đình
- Lớp: CNTT 17-08
- Vai trò/Service phụ trách: A4 - AI Vision Service
- Sản phẩm: Product A - Smart Campus Operations Platform
- Hệ điều hành: Windows, PowerShell
- Môi trường Python: conda `api-platform`, Python 3.11.15

## Đề tài A4

- Service phụ trách: AI Vision
- Tên đề tài: Xây dựng dịch vụ AI phân tích hình ảnh
- Bối cảnh ứng dụng: môi trường giáo dục thông minh khép kín

## Các file minh chứng cần có

- [x] `README.md`
- [x] `checklist.md`
- [x] `known-issues.md`
- [x] `tool-versions.txt`
- [x] `docker-version.txt`
- [x] `compose-version.txt`
- [x] `hello-world.txt` - đã có file ghi trạng thái hiện tại, cần chạy lại Docker để có output thành công
- [x] `smoke-test-result.txt` - đã có file ghi trạng thái hiện tại, cần chạy lại smoke test khi Docker daemon sẵn sàng
- [x] `image-list.txt` - đã có file ghi trạng thái hiện tại, cần chạy lại Docker image list khi Docker daemon sẵn sàng
- [x] `git-log.txt`
- [x] `service-boundary.md`

## Lệnh chạy lại khi Docker Desktop sẵn sàng

```powershell
$env:PATH = "C:\Program Files\Docker\Docker\resources\bin;C:\Users\tungb\anaconda3\envs\api-platform;C:\Users\tungb\anaconda3\envs\api-platform\Scripts;$env:PATH"
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
.\scripts\collect_session01_evidence.ps1
```
