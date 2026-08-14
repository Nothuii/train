# Nhiệm vụ 
tìm pass trong file -
# Thực hiện
sau khi đã có có được pass để vào bandit 1 thì ta dùng lệnh 
```bash
exit
``` 
để thoát ra 
Và sau đó sử dụng tiếp tục sử dụng câu lệnh ssh 
```bash 
ssh -p 2220 bandit1@bandit.labs.overthewire.org 
``` 
để truy cập vào `bandit1`
Ta lại sử dụng lệnh 
```bash
ls 
```
khi này nó hiện ra file có tên 
```bash 
-
```
Tuy nhiên khi này nếu ta sử dụng `cat -` thì sẽ không đọc được do khi này nó sẽ hiểu thành `STDIN`
Để tránh xảy ra ta phải sử dụng 
```bash 
cat ./-
```
Thì khi này máy sẽ hiểu là ta cần đọc file tên - 
# Password 
```bash 
6y2kwnwK6grgvwvpvLaa2T1cpFEKOhNR
``` 