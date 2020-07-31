# Chương VI


trình soạn thảo văn bản
có 2 chế độ: comand và insert

![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/1.png)



## vào chế độ insert

* a bắt đầu ngay sau kí tự đang chọn
* A bắt đầu tại cuối dòng đang chọn
* i bắt đầu ngay trước kí tự đang chọn
* I Bắt đầu tại đầu dòng đang chọn
* o Bắt đầu tại 1 dòng mới ngay dưới dòng đang chọn
* O Bắt đầu tại 1 dòng mới ngay trên dòng đang chọn
  

ví dụ: kí tự đang chọn là `e` dòng 2

![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/2.png)


|Command | Action|
:---------:|:---------|
a |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/3.png)
A |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/4.png)
i |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/5.png)
I |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/6.png)
o |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/7.png)
O |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/8.png)

## thay thế, xoá kí tự

* x xoá kí tự ngay tại con trỏ chuột
* X xoá kí tự ngay trước con trỏ chuột
* r thay thế kí tự ngay tại con trỏ chuột ( sau đó nhập kí tự mới)
* p dán kí tự ngay sau con trỏ chuột (kí tự xoá cuối cùng)
* xp thay đối 2 kí tự với nhau
  

|Command | Action|
:---------:|:---------|
x |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/9.png)
X |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/10.png)
r |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/11.png)
p |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/12.png)
xp |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/13.png)

## undo

`u` : undo 

## cắt, sao chép, dán dòng


1. `v` (hoặc `V` nếu bạn muốn cut cả dòng).
2. Di chuyển con trỏ đến vị trí cuối đoạn văn bản muốn cut
3. Bấm `d`
   

* yy (yank yank) sao chép dòng hiện tại
* p dán dòng vừa sao chép ngay dưới dòng hiện tại
* P dán dòng vừa sao chép ngay trên dòng hiện tại

|Command | Action|
:---------:|:---------|
yy |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/14.png)
p |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/15.png)
P |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/16.png)


cut hoặc coppy nhiều dòng thêm số (dòng)

* 3V: cut 3 dòng bắt đầu từ dòng hiện tại
* 4yy: copy 4 dòng bắt đầu từ dòng hiện tại


## bắt đầu và kết thúc của dòng

* 0 hoặc ^: nhảy đến đầu dòng
* $ :       nhảy đến cuối dòng
* d0:  xoá đến đầu dòng
* d$:  xoá đến cuối dòng

|Command | Action|
:---------:|:---------|
0 hoặc ^ |  ![line](https://github.com/minhvl/linux/blob/trainning/image/VI/17.png)
$ |  ![line](https://github.com/minhvl/linux/blob/trainning/image/VI/18.png)
d0 |  ![line](https://github.com/minhvl/linux/blob/trainning/image/VI/19.png)
d$ |  ![line](https://github.com/minhvl/linux/blob/trainning/image/VI/20.png)

## nối 2 dòng lien tiếp
`J`

![line](https://github.com/minhvl/linux/blob/trainning/image/VI/21.png)


`yyp` nhân đôi dòng

![line](https://github.com/minhvl/linux/blob/trainning/image/VI/22.png)


## cắt, xoá, sao chép từ


* w nhảy tới từ tiếp theo
* b lùi lại từ trước đó
* 3w nhảy tới 3 từ tiếp theo
* dw xoá 1 từ
* yw sao chép 1 từ
* 7dw xoá 7 từ


|Command | Action|
:---------:|:---------|
w  |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/23.png)
b  |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/24.png)
dw |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/25.png)
yw |  ![vi](https://github.com/minhvl/linux/blob/trainning/image/VI/26.png)


## lưu, thoát

* :w save (write)
* :q quit
* :wq save and quit
* ZZ save and quit
* :q! quit (discarding your changes)

## tìm kiếm
