# DOCKER
## thành phần
- images
- container

## Images

*Kiểm tra các images hiện có*

`docker images` 


*tải images, nếu không kèm tag mạc định tải Version lates*
`docker pull "tên images:tag"`  

*xoá images*
`docker rm "tên images"`

`docker rm " ID images"`

## container

*thực thi images/ khởI tạo container*

`docker run -it "tên images / ID images"`
> -i tương tác
> -t dùng terminal


`docker run -it --name " tên container" -h "hostname images"`

>
>
*thoát container*

`docker exit`


*kiểm tra container đang chạy*

`docker ps`


*tất cả container*

`docker ps -a`


*thoát container mà k làm dừng*

**ctrl + p +q**


*dừng container*

`docker stop "container id"`



*start container*

`docker start "container id"`



*vào terrminal container đang chạy*

`docker attach " container id"`
