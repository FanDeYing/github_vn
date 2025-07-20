# Terms

Repository (Repo):
 => Kho chứa toàn bộ mã nguồn và lịch sử thay đổi. Có thể là local (trên máy bạn) hoặc remote (trên GitHub, GitLab...)                                            
Branch:
 =>	Nhánh phát triển độc lập của mã nguồn. Mỗi branch giống như một bản sao để thử nghiệm, phát triển tính năng.
Conflict:
 => Xung đột xảy ra khi Git không thể tự quyết định giữ phần thay đổi nào giữa 2 nhánh. Bạn phải chỉnh sửa thủ công.
Local:
 => Dự án Git nằm trên máy tính cá nhân của bạn. Chưa được đưa lên mạng.
Remote:
 => Dự án Git nằm trên dịch vụ như GitHub/GitLab. Bạn cần push để gửi mã từ local lên remote.

# Commands

- git init:
=> Khởi tạo Git trong thư mục hiện tại (tạo thư mục .git)

- git status:
=> 	Kiểm tra trạng thái tệp đã thay đổi, chưa theo dõi hoặc đã staged

- git add:
=> Thêm tệp vào khu vực chờ để commit (staging area). VD: git add index.html

- git reset:
=> Bỏ tệp ra khỏi khu vực staging. Không xóa file!

- git commit:
=> Ghi lại những thay đổi vào lịch sử Git. VD: git commit -m "Lời nhắn"

- git log:
=> Hiển thị lịch sử các commit

- git log --oneline:
=> Hiển thị lịch sử commit dưới dạng ngắn gọn, mỗi commit 1 dòng

- git checkout {branch name}:
=> Chuyển sang nhánh {branch} đã tồn tại

- git branch:
=> Liệt kê các nhánh hiện có

- git checkout -b {branch name}:
=> Tạo và chuyển sang nhánh mới tên {branch}

- git merge {branch name}:
=> Gộp nhánh {branch} vào nhánh hiện tại

- git branch -d {branch name}:
=> Xóa nhánh {branch} (chỉ khi đã merge)

- git push:
=> Đẩy commit từ máy local lên remote (thường là GitHub)

- git remote add origin {Repo url}:
=> Liên kết repo local với repo từ xa (remote). origin là tên mặc định cho remote

- git fetch origin:
=> Lấy các thay đổi mới từ remote về máy local (chưa hợp nhất)

- git checkout -b {branch name} origin/{branch name}:
=> Tạo nhánh local từ nhánh remote (theo dõi nhánh từ xa)