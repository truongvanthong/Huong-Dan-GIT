# Hướng dẫn sử dụng GIT

## Mục lục
- [1. Cài đặt GIT Bash](#1-cài-đặt-git-bash)
- [2. Cấu hình GIT](#2-cấu-hình-git)
- [3. Tạo repository](#3-tạo-repository)
- [4. Các lệnh cơ bản](#4-các-lệnh-cơ-bản)
- [5. Branch](#5-branch)
- [6. Sử dụng GitHub Desktop](#6-sử-dụng-github-desktop)

---

## 1. Cài đặt GIT Bash
- Truy cập trang chủ của GIT: [https://git-scm.com/](https://git-scm.com/)
- Tải bản cài đặt phù hợp với hệ điều hành của bạn.

## 2. Cấu hình GIT
- Mở GIT Bash lên và thực hiện các lệnh sau:
    + Cấu hình tên và email: 
    ```bash
    git config --global user.name "Tên của bạn"
    git config --global user.email "Email của bạn"
    ```
    + Kiểm tra thông tin đã cấu hình:
    ```bash
    git config --list
    ```

## 3. Tạo repository
- Tạo repository trên trang [GitHub](github.com)

- Cách 1: Clone repository đã tồn tại
    ```bash
    git clone <URL của repository>
    ```
- Cách 2: Tạo repository mới
    ```bash
    git init
    ```
    + Tạo file README.md
    ```bash
    echo "# Tên repository" >> README.md
    ```
    + Thêm file README.md vào staging area
    ```bash
    git add README.md
    ```
    + Commit file README.md
    ```bash
    git commit -m "Thêm file README.md"
    ```
    + Đẩy file README.md lên repository
    ```bash
    git remote add origin <URL của repository>
    git push -u origin master
    ```
## 4. Các lệnh cơ bản
- Xem trạng thái của repository
```bash
git status
```
- Thêm file vào staging area
```bash
git add <Tên file>
```
- Commit file
```bash
git commit -m "Nội dung commit"
```
- Đẩy file lên repository
```bash
git push
```
- Cập nhật repository
```bash
git pull
```
- Xem lịch sử commit
```bash
git log
```
- Xem lịch sử commit theo định dạng đẹp hơn và ngắn gọn
```bash
git log --oneline --graph
```
- Xem lịch sử commit của một file
```bash
git log <Tên file>
```

## 5. Branch
- Xem tất cả các branch
```bash
git branch
```
- Tạo branch mới
```bash
git branch <Tên branch>
```
- Chuyển sang branch khác
```bash
git checkout <Tên branch>
```
- Tạo branch mới và chuyển sang branch đó
```bash
git checkout -b <Tên branch>
```
- Merge branch
```bash
git merge <Tên branch>
```
- Xóa branch
```bash
git branch -d <Tên branch>
```

## 6. Sử dụng GitHub Desktop    
- Tải GitHub Desktop tại: [https://desktop.github.com/](https://desktop.github.com/)