![thrfhtrhdtrthrththhtdf](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/76274f83-8329-4b36-8262-a183ad3c7341)

Preliminary testing for creating infrastructure servers for MPO+ NA/US version (ULUS10290)
With "PPSSPP infra build" to use PrimaryDNS in PPSSPP.ini

You can download it there: https://www.mediafire.com/file/h3uzx13g4iqmsqo/PPSSPP_1.13.1-18+infra_win.rar/file

First im using wireshark (not master version because filters doesn't work) with the game on "localhost" to found and trigger informations from client to -> server

Then spotted differents things that the client (game) try to do ;

1. game try to make several DNS check with the previous stun Server : mpostunus.konamionline.com (doesn't exist since May 2012)
2. Then try to found the page with "terms of use" that you had to accept at : http://info.service.konamionline.com/VP029-U1/info/ (doesn't exist since May 2012)
3. It will try to connect to "HTTPS" to found accounts, user names, password, games settings, etc.. at : https://mpoweb.konamionline.com/us/mpo/ (doesn't exist since May 2012) (Maybe need to affiliate to the ip of actual server then redirect the "HTTP" URL via cheat that is in the PPSSPP infra build upside)
4. Then it will set you up to a "Server Lobby" on NA US version we have "gate02", Jap it's "gate01", EU is "gate03" at : mpogate02.konamionline.com (doesn't exist since May 2012)
5. Normally after all of that game/client is connected to server, maybe gonna need to do more with other pages (Ranking, join host, create host, etc...)

Some screens from the official servers (sorry it's in french) 

After this page that we still actually could access the game check the stun server make some DNS check and result today to an UDP error (P518)

![2](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/7114c37e-d47f-4d8a-9ac4-f8be32fd75ff)


Therms of use page we had to accept that the client try to read on http://info.service.konamionline.com/VP029-U1/info/

![5](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/2d0c66d1-a802-4574-90d2-b18eada313be)


Session account (Open, create, change passwords, etc...) where the game will catch them on the URL https://mpoweb.konamionline.com/us/mpo/

![6](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/ed10ed11-4715-49e8-bca3-b5d8e89c6f49)


Then the game search about the "gate" i explained upside 

![11](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/3fafe8fb-9918-4701-8c7d-781e1dabcb48)


and after choose a Lobby server there we are : 

![15](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/dc6f715c-49c3-41e0-8b76-704f4b126fef)

With different pages like join, create host, ranking etc...


Ranking was like that : 

![16](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/285059a3-b85f-4c1a-9cf1-bcb2c0022a21)


Then you could select one player to see the personal ranking page :

![17](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/967c9898-38c7-4a3e-ac41-f67d84563be4)
![18](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/6b71f085-b02e-4bb6-8a2c-03ebc7c69edc)
