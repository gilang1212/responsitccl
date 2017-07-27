# responsitccl

![2.PNG](https://github.com/gilang1212/gilang/blob/master/2.png)
### Create Dockerfile :

FROM nginx:alpine

COPY index.html /usr/share/nginx/html/index.html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]

### penjelasan code pada Dockerfile :

● FROM : mendefenisikan base image Docker yang digunakan, dalam contoh ini menggunakan nginx:alpine 

● COPY melakukan proses duplikasi file index.html pada direktori imageku ke dalam root direktori nginx di dalam container

● EXPOSE : Mendefenisikan port yang digunakan 

● CMD : Eksekusi perintah command pada lingkungan container 

### Proses :

$mkdir tccl

$cd tccl

$ docker build -t gilang:v1
![33.PNG](https://github.com/gilang1212/gilang/blob/master/33.png)

$ docker run -d -p 80:80 gilang:v1

$docker run -p 8080:80 --name gilang-1 gilang



