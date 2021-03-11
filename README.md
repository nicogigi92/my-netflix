__my-netflix__  

Here is my docker and traefik config files. They allow to run a seedbox on a remote server, with an emby app to watch your content remotely.   

My config :  
  Debian 9.0
  Docker 19.03.15  
  Docker-compose 1.28.5   
  
If you want to make it run on your own server you will have to download and install docker and docker-compose.  
https://docs.docker.com/engine/install/debian/  
https://docs.docker.com/compose/install/  

You also need DNS pointing on your server :  
  
  www.mydns.ex  
  emby.mydns.ex  
  torrent.mydns.ex  
  web.mydns.ex  

After cloning the repo, you will have to adapt few things in files :  

Change *mydns.ex* by your own dns.  
Put your *email* adress for acme challenge (letsencrypt certificate).  
Add your ip adress into the ip whitelist.  

Maybe you will have to create two directories :  
  
  mkdir rutorrent  
  mkdir traefik_letsencrypt  
