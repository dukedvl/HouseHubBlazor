# HouseHub Blazor

![image](https://github.com/dukedvl/HouseHubBlazor/assets/9894325/0e5f5da1-a170-429e-a181-a419ad945049)

![image](https://github.com/dukedvl/HouseHubBlazor/assets/9894325/cf408295-523d-4e8b-8b7f-ca9f39f0608e)

```
docker build -t househubblazor:alpine .      //build img
docker run -p 8080:80 househubblazor:alpine   //run img, testing locally

docker save househubblazor:alpine -o blazor.tar   //export img off dev machine

sftp put blazor.tar //(sftp the image over to the linux box)

sudo docker load -i blazor.tar   //import the image file
sudo docker run -p 3032:80 --name househub_blazor househubblazor:alpine  //run it on the server!
```
