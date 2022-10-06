# Use-Github-and-Git

## Các thuật ngữ nên biết

### Working directory, staging area, repository và local repo
- **Working directory**: là nơi mà các file mới được tạo, file cũ bị xóa hoặc là nơi thực hiện các thay đổi đối với các file đã có. Tóm lại khi tạo  một project rồi gõ `git init` hoặc clone một repo về thì sẽ có folder tên là `.git` thì mọi thao tác thêm, sửa, xóa file trên folder đó thì coi như đang thực hiên trên **working directory**
- **Staging area**: sau khi hoàn tất các thao tác trên file ở **working directory** thì thêm các file này vào trong **staging area** bằng lệnh `git add`. Rất rõ ràng **Stagin area** là nơi lưu trữ các thay đổi trước khi `commit`.
- **Repository**: hiểu đơn giản là nơi lưu tất cả các thông tin cần thiết để duy trì quản lý các đổi và lịch sử của toàn bộ project. Túm lại là sau khi `git commit`thì các thay đổi được lưu ở đây. Tất cả dữ liệu của Repository đều được chứa trong **working directory** dưới dạng folder `.git`. Repo có 2 loại: `remote repo` và `local repo`. 
- **Remote rep**: là rep để chia sẽ nhiều người
- **Local repo**: là rep trên máy dev của chúng ta, dành cho một người dùng
## Các lệnh Git cơ bản

### 1. Git init
* Công dụng: Để tạo kho lưu trữ (repository) và 1 dự án mới
* Sử dụng: trong thư mục gốc của dự án<br>
`git init`

### 2. Git add
* Công dụng: Thêm các file vào stage. Có thể thêm toàn bộ thư mục hoặc các file cụ thể
* Sử dụng: `git add <file or directory name>` hoặc `git add .` để add tất cả các file 

### 3. Git commit
* Công dụng: Để ghi lại những thay đổi được thực hiện với file vào **local repo**. Để dễ dàng theo dõi commit và mỗi commit đề có mã id duy nhất
* Sử dung: `git commit -m "Commit message"`

### 4. Git status
* Công dụng: nếu file nằm trong **stagging area** mà chưa được commit thì sẽ hiện thị ra.
* Sử dụng: `git status`

### 5. Git branch
* Công dụng: xác định nhánh nào trong local rep, thêm hoặc xóa một nhánh mới
* Sử dụng: <br>
  * Tạo một nhánh mới: `git branch <branch_name>`<br>
  * Danh sách các branch remote hoặc local: `git branch -a`<br>
  * Xóa một nhánh: `git branch -d <branch_name>`
  
### 6. Git checkout
* Công dụng: dùng để chuyển đổi các nhánh
* Sử dụng: `git checkout <branch_name>`

### 7. Git merge
* Công dụng: hợp nhất các nhánh với nhau
* Sử dụng: `git merge <branch_name>`

### 8. Git remote
* Công dụng: để kết nối repo với kho lưu trữ từ xa
* Sử dụng: khi mới tạo repo trên Github sẽ có dành git git remote

### 9. Git clone
* Công dụng: để sao chép và tải repo về máy tính
* Sử dụng: `git clone <remote_URL`

### 10. Git pull
* Công dụng: kéo code từ repo sang máy tính
* Sử dụng: `git pull <branch_name>/<remote_URL/remote_name `

### 11. Git push
* Cộng dụng: dùng để gửi commit đến remote repo
* Sử dụng: `git push <remote_URL/remote_name> <branch>`
