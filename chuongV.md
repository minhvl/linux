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