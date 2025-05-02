# html-doraemon
HTML Doraemon

# git 
*** git clone***
dùng để kéo repo từ gihub về
```bash
    git clone <url>
```

*** lệnh cơ bản git push lên***
```bash 
git status
git add .
git commit -m "ghi chu"
git push origin tên_nhánh
```

*** lệnh kéo về ***
```bash
git pull origin tên_nhánh
```

*** tạo nhánh mới ***
git checkout -b tên_nhánh

*** xóa nhánh ***
git branch -d tên_nhánh

*** git merge nhánh ***
git merge tên_nhánh 

*** quy trình xử ly conflict ***
khi merge nhánh con ( nhánh đang làm vào nhánh chính (ex: dev, masterr,...))
bị conflict

thì chúng ta xử lý như sau:
ex: đang làm trên nhánh feat/tran_1
muốn merge qua nhánh dev
đang đứng trên nhanh feat/tran_1

git checkout dev
git pull origin dev
git checkout feat/tran_1
git merge dev

code . ( mở vs code xử lý)

sau đó đẩy lên ( bộ git push )

*** git stash ***
trường hợp đang làm nhiều người trên nhánh hoặc nhiều máy thì lỗi lịch sử commit hoặc lỗi push lên nhiều phân đoạn ta cần lưu lại code hiện tại như sau:

```bash
git stash
git pull origin tên_nhánh ( đang làm)
git stash pop

```
