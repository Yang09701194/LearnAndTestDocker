# LearnAndTestDocker

1- Follow https://docs.docker.com/docker-for-windows/ install Docker on Windows. 

2- Follow step in [Learn Docker in 12 Minutes 🐳](https://www.youtube.com/watch?v=YFl2mCHdv24) 

3- Got Error: [no matching manifest for windows/amd64 in the manifest list entries](https://stackoverflow.com/questions/48066994/docker-no-matching-manifest-for-windows-amd64-in-the-manifest-list-entries) 

I guess it's because many package only support docker on linux, but not support docker on windows, so I want to make a linux OS with docker.

4- Turn to test on Linux Docker, first [Install CentOS](http://blog.itist.tw/2014/07/centos7-prepare.html)

5- Then I first try [Docker Official Tutorial: Get Docker CE for CentOS](https://docs.docker.com/install/linux/docker-ce/centos/) <br/> 
, but in the step `sudo yum install docker-ce`, I got error `No package docker-ce available. `.

6- I find another [CentOS install Docker tutorial : 
001-在 Cent OS 7 上安装 docker-ce]() works, and install Docker successfully


### Virtualbox Network Connect from Hosr to Guest Virtual CentOS Machine

* Related Link
  * https://gist.github.com/odan/48fc744434ec6566ca9f7a993f4a7ffb
  * https://serverfault.com/questions/225155/virtualbox-how-to-set-up-networking-so-both-host-and-guest-can-access-internet
* My Setting
  * Adpater1  NAT, Adapter2 Host-only + Advanced - Allow All
  * ![alt text](https://i.imgur.com/Ync4chK.png)
* After turn on the OS, use `ifconfig` to show the network information, by my test the correct IP position is in `np0s8`
  * ![alt text](https://i.imgur.com/dlyXQJK.png)
  
  
