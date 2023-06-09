# LinuxCommand
Common Linux command (Linux &amp; WSL)

### ls
* ls

* ls -a

* ls -l

* ls -la

* ls -R

h: Hiển thị dung lượng của thư mục vào file con

a: Hiển thị các file ẩn trong thư mục

l: List toàn bộ thông tin của file lần lượt là quyền, người sở hữu, nhóm sở hữu, kích cỡ của file, thời gian và tên file

### cd
change directory: di chuyển đến thư mục đích

### clear
clear screen

### mkdir
Make directory

Tạo hàng loạt thư mục: mkdir -p parent/children1/children2

### rmdir <dir>
  Xóa thư mục trống

Lệnh xóa thư mục có file: rm -r

### rm <file>
  
Xóa file

### touch
Tạo 1 file

ví dụ: touch test.html
  
### vi

mở file trong Vim
  
* Insert mode tại vị trí con trỏ: a

* Normal mode: ESC

* Lưu file: :w

* Thoát nhưng không lưu: :q

* Thoát có lưu file: :wq

Thêm ! cuối lệnh không lưu file nếu có thay đổi trong file
  
https://itplusx.info/su-dung-vim-co-ban-toi-nang-cao/

### cat
ghi ra nội dung các file sau cat nối tiếp nhau
nếu có dấu > <file> -> ghi ra file mới

### echo
in nội dung

  vd:
  echo "Hello"
  echo "Hello bro" > test.html
  
### tail
  in ra những dòng mới nhất (10) trong file
  
  tail test.html
  
  tail -n 20 test.html
  
  tail -f test.html -> khi file thay đổi thì tự in ra

### grep
  https://tenten.vn/tin-tuc/lenh-grep-la-gi/
  
  Tìm kiếm chuỗi trong một file
  grep "chuỗi cần tìm" tên_file
  
  Tìm kiếm chuỗi sử dụng biểu thức chính quy (regular expression)
  grep -E '^a' example.txt
  
### cp
  copy file
  
  cp [additional_option] source_file target_file
  
  [doc](https://lanit.com.vn/cach-su-dung-lenh-copy-trong-linux-bang-vi-du-de-hieu.html)
  
### mv
  đổi tên/ di chuyển
  
### rm
  xóa file/ folder(-r)
  
  Chú ý rmdir chỉ xóa được thư mục trống, do đó khi xóa thư mục hay dùng rm -r <dir>
