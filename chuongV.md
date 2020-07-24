# V: pipe and command


## tac

in ra các dòng của file theo thứ tự từ dưới lên trên ( ngược với `cat`)

![cat](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/1.png)

![tac](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/2.png)

## tee
chuyển hướng dữ liệu stdout vào file ( tương tự như `>` kết hợp `ls`)

![tee](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/3.png)

sử dụng option `-a` để không ghi đè lên dữ liệu có sẵn

>
![tee](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/4.png)

> những stderr sẽ không được `tee` chuyển hướng
> 
> nếu muốn ghi stdeer,chuyển stderr thành stdout `2>&1`

_`1>&2` chuyển stdout thành stderr_

![tee](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/5.png)

## grep

![](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/6.png)


![](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/7.png)

`grep` thường kết hợp với lệnh `cat`



* `grep -i` không phân biệt chữ hoa , thường
* `grep -v` lọc tất cả kết quả không giống từ khoá đang chọn
* kết hợp cả 2 `grep -vi` 

![](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/8.png)



* `grep -A1` hiển thị 1 dòng ngay dưới kết quả tìm dc
* `grep -B1` hiển thị 1 dòng ngay trên kết quả tìm dc
* `grep -C1` hiển thị 1 dòng ngay trên và dưới kết quả tìm dc
* có thể thay đổi số dòng hiển thị ngay sau chữ A,B,C ví dụ: A2, B10, C200

![](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/9.png)

## tr

**translate**

thay thế hoặc xoá kí tự

![tr](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/10.png)

thay thế n thành N


chuyển tất cả kí tự in thường thành hoa và ngược lại
![tr](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/11.png)


xoá kí tự 'h'
![tr](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/12.png)


## sort

**mặc định sắp xếp theo a->z**

![sort](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/13.png)



sắp xếp theo cột thứ 2 dùng option `-k[số cột]`

![tr](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/14.png)



muốn sắp xép theo chữ số dùng option `-n`

![tr](https://github.com/minhvl/linux/blob/trainning/image/New%20folder/15.png)




