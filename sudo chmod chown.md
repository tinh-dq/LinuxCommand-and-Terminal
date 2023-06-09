### sudo
thực hiện dòng lệnh với quyền super user, tài khoản root

### chmod
change mode: 
sửa đổi quyền đọc, ghi và thực thi của tệp hoặc thư mục.

Có 3 lớp người dùng: chủ sở hữu (user), thành viên nhóm (group) và các lớp khác (other)

vd: chmod [tùy chọn] [quyền] [file_name]

*Giải thích:*

r: read, w: write, x: excecute

-> dùng hệ bát phân để phân quyền (0-7)
vd: 777

### chown
thay đổi quyền sở hữu tệp, thư mục hoặc liên kết tượng trưng thành tên người dùng được chỉ định.

chown [option] owner[:group] file(s)

vd: chown linuxuser2 file_name.txt
