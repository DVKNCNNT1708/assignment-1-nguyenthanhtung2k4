# Checklist Buổi 1

Đánh dấu theo trạng thái thực tế tại thời điểm kiểm tra.

## Công cụ

- [x] Git đã cài và chạy được `git --version`.
- [x] Docker CLI đã cài và chạy được `docker --version`.
- [ ] Docker daemon chưa kiểm tra thành công do `\\.\pipe\docker_engine` bị `Access is denied`.
- [x] Docker Compose CLI đã cài và chạy được `docker compose version`.
- [x] Node.js đã cài và chạy được `node --version`.
- [x] npm đã cài và chạy được `npm --version`.
- [x] Python/Miniconda đã cài và env `api-platform` chạy được Python 3.11.15.
- [x] VS Code đã cài.
- [x] Postman đã cài.

## Docker

- [ ] `docker run --rm hello-world` chưa có output thành công trong evidence.
- [ ] Chưa xác nhận đã chạy xong `scripts/pull_all.ps1`.
- [ ] `scripts/smoke_test.ps1` chưa chạy xong do Docker daemon chưa sẵn sàng.
- [ ] Mini-stack Docker Compose chưa kiểm tra thành công.

## GitHub

- [x] Đã clone repo lớp về máy.
- [x] Branch Buổi 1: không bắt buộc nếu giảng viên không yêu cầu.
- [x] Chưa commit minh chứng Buổi 1 sau lần cập nhật này.
- [x] Chưa xác nhận đã push lên GitHub.

## OBE Evidence

- [x] `evidence/buoi-01/README.md` có nội dung.
- [x] `evidence/buoi-01/checklist.md` có nội dung.
- [x] `evidence/buoi-01/known-issues.md` có nội dung.
- [x] `evidence/buoi-01/tool-versions.txt` có nội dung.
- [x] `evidence/buoi-01/docker-version.txt` có nội dung.
- [x] `evidence/buoi-01/compose-version.txt` có nội dung.
- [x] `evidence/buoi-01/hello-world.txt` có nội dung ghi trạng thái hiện tại.
- [x] `evidence/buoi-01/smoke-test-result.txt` có nội dung ghi trạng thái hiện tại.
- [x] `evidence/buoi-01/image-list.txt` có nội dung ghi trạng thái hiện tại.
- [x] `evidence/buoi-01/git-log.txt` có nội dung.
- [x] `evidence/buoi-01/service-boundary.md` đã mô tả đề tài A4 - AI Vision.

## Việc cần làm tiếp

1. Mở Docker Desktop và chờ đến khi trạng thái running.
2. Nếu vẫn bị `Access is denied`, mở PowerShell bằng Run as administrator.
3. Chạy lại `.\scripts\collect_session01_evidence.ps1`.
4. Kiểm tra lại checklist sau khi các file Docker log đã có output thành công.
5. Commit và push sau khi Docker chạy lại thành công hoặc sau khi giảng viên chấp nhận ghi chú lỗi hiện tại.
