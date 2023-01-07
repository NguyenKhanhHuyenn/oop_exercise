# oop_exercise
# **GIT**

1. **Git là gì?**

Git là một hệ thống quản lý phiên bản phân tán (Distributed Version Control System – DVCS), nó là một trong những hệ thống quản lý phiên bản phân tán phổ biến nhất hiện nay. Git cung cấp cho mỗi lập trình viên kho lưu trữ (repository) riêng chứa toàn bộ lịch sử thay đổi.

2. **Version Control System – VCS là gì?**

VCS là viết tắt của Version Control System là hệ thống kiểm soát các phiên bản phân tán mã nguồn mở. Các VCS sẽ lưu trữ tất cả các file trong toàn bộ dự án và ghi lại toàn bộ lịch sử thay đổi của file. Mỗi sự thay đổi được lưu lại sẽ được và thành một version (phiên bản).

VCS giúp bạn có thể lưu trữ nhiều phiên bản khác nhau của một mã nguồn được nhân bản (clone) từ một kho chứa mã nguồn (repository), mỗi thay đổi vào mã nguồn trên local sẽ có thể server nơi đặt kho chứa chính.

Mỗi phiên bản bao gồm: nội dung file bị thay đổi, ngày giờ sửa đổi, người thay đổi là ai, lý do thay đổi hay tên phiên bản, …

3. **Các thuật ngữ Git quan trọng**

**3.1 Branch**

- Các Branch (nhánh) đại diện cho các phiên bản cụ thể của một kho lưu trữ tách ra từ project chính của bạn.
- Branch cho phép bạn theo dõi các thay đổi thử nghiệm bạn thực hiện đối với kho lưu trữ và có thể hoàn nguyên về các phiên bản cũ hơn.

**3.2 Commit**

Một commit đại diện cho một thời điểm cụ thể trong lịch sử dự án của bạn. Sử dụng lệnh commit kết hợp với lệnh git add để cho git biết những thay đổi bạn muốn lưu vào local repository.

**3.3 Head**

Các commit ở đầu của một branch được gọi là head. Nó đại diện cho commit mới nhất của repository mà bạn hiện đang làm việc.

**3.4 Master**

- Master là nhánh chính của tất cả các repository của bạn. Nó nên bao gồm những thay đổi và commit gần đây nhất.
- Đối với github nhánh chính là main

**3.5 Origin**

Origin là phiên bản mặc định của repository. Origin cũng đóng vai trò là bí danh hệ thống để liên lạc với nhánh chính.

Lệnh git push origin master để đẩy các thay đổi cục bộ đến nhánh chính.

**3.6 Remote**

Một Remote (kho lưu trữ từ xa) là một bản sao của một chi nhánh. Remote giao tiếp ngược dòng với nhánh gốc (origin branch) của chúng và các Remote khác trong kho lưu trữ.

**3.7 Repository**

Kho lưu trữ Git chứa tất cả các tệp dự án của bạn bao gồm các branch, tags và commit.

**3.8 Tags**

Tags cung cấp cho bạn một cách để theo dõi các commit quan trọng. Các tags nhẹ chỉ đơn giản đóng vai trò là con trỏ trong khi các tags chú thích được lưu trữ dưới dạng các đối tượng đầy đủ.

4. **Các lệnh cơ bản trong git**

**4.1. git config**

Câu lệnh để set user name và email của bạn trong main configuration file.

Để kiểm tra tên và kiểu email trong cấu hình dùng git config -- global user.name và git config -- global user.email

**4.2. git init**

Dùng để khởi tạo 1 git repository 1 project mới hoặc đã có.

**4.3. git clone**

Dùng để copy 1 git repository từ remote source.

Câu lệnh: git clone \<:clone git url:\>

**4.4. git status**

Kiểm tra trạng thái của những file bạn đã thay đổi trong thư mục làm việc.

Câu lệnh: git status trong thư mục làm việc.

**4.5. git add**

Thêm thay đổi đến stage/index trong thư mục làm việc.

Câu lệnh: git add

**4.6. git commit**

Commit là một action để Git lưu lại một snapshot của các sự thay đổi trong thư mục làm việc. Và các tập tin, thư mục được thay đổi đã phải nằm trong Staging Area. Mỗi lần commit nó sẽ được lưu lại lịch sử chỉnh sửa của code kèm theo tên và địa chỉ email của người commit. Ngoài ra trong Git bạn cũng có thể khôi phục lại tập tin trong lịch sử commit của nó để chia cho một branch khác, vì vậy bạn sẽ dễ dàng khôi phục lại các thay đổi trước đó.

Câu lệnh: git commit -m "message"

**4.7. git push/git pull**

Tác dụng: Push hoặc Pull các thay đổi đến remote. Nếu bạn đã added và committed các thay đổi và bạn muốn đẩy nó lên hoặc remote của bạn đã update và bạn apply tất cả thay đổi đó trên code của mình.

Câu lệnh: _git pull \<:remote:\> \<:branch:\>_ và _git push \<:remote:\> \<:branch:\>_

5. **Quy trình làm việc git cơ bản**

- git init – Tạo 1 repository
- git status - Đảm bảo răng local của bạn đang sạch sẽ.
- git pull - Tải phiên bản code mới nhất từ remote.
- Chỉnh sửa các tệp của bạn.
- git status - Tìm kiếm tất cả các file đã được thay đổi.
- git add [file] - Thêm các tệp tin thay đổi vài stage changes.
- git committ -m "message" - Thực hiện commit của bạn.
- git push origin - đẩy thay đổi của bạn lên remote.

6. **GitHub**

GitHub là một dịch vụ nổi tiếng cung cấp kho lưu trữ mã nguồn Git cho các dự án phần mềm. Github có đầy đủ những tính năng của Git, ngoài ra nó còn bổ sung những tính năng về social để các developer tương tác với nhau.

GitHub  **cung cấp các tính năng social networking**  như feeds, followers, và network graph để các developer học hỏi kinh nghiệm của nhau thông qua lịch sử commit.
