# Chương VII: Scrip


Tạo 1 file scipt đơn giản

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/1.png)


để chạy file .sh sử dụng `./filename` hoặc ` bash filename`



## she-bang

> Shebang (hay sha-bang, hashbang, pound-bang, hash-pling) là kí tự `!#` , nó luôn được đặt ở dòng đầu tiên trong mỗi script. Trong hệ thống UNIX/LINUX, mỗi khi 1 script được chạy, đầu tiên program loader sẽ dựa vào Shebang để xác định script sẽ được thực thi bởi trình biên dịch nào. Nếu 1 script không có Shebang thì mặc định nó sẽ được thực thi bởi Sh.


Bash shell

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/2.png)


Korn shell

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/3.png)

## Comment

sau kí tự `#` : là comment

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/4.png)


## Biến

Gọi biến dùng kí tự `$`

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/5.png)


## Sourcing script

gọi các biến có trong file script ở cùng shell

sử dụng `source ./filename` hoặc `. ./filename`


![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/6.png)


## troubleshooting

`bash -x` xem các lệnh mà shell thực thi

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/7.png)


## Test

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/8.png)


có thể viết thành `true` và `false`

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/9.png)



câu lệnh `test` có thể  viết là ` []`

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/10.png)



kết hợp với các phép toàn login `-a` (and) ; `-o` (or)


![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/11.png)


## if then else

Script kiểm tra file `1.txt` có tồn tại ko?

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/12.png)

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/13.png)



## if then elif

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/14.png)


## for loop


![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/15.png)

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/16.png)

lặp lại câu lệnh echo cho tới khi in ra hết kết quả



![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/17.png)

biến là 1 dãy số tự nhiên liên tiếp nhau



## while loop

đếm ngược từ 10 về 0


![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/18.png)

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/19.png)


## until loop

_Ngược lại while loop_

![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/20.png)


![vii](https://github.com/minhvl/linux/blob/trainning/image/VII/21.png)


