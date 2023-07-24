![thrfhtrhdtrthrththhtdf](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/7adc8831-199e-4371-8a86-0afb8f2fe61c)


Preliminary testing for creating infrastructure servers for MPO+ NA/US version (ULUS10290)
With "PPSSPP infra build" to use PrimaryDNS in PPSSPP.ini

You can download it there: https://www.mediafire.com/file/r5ir0k682pt9a78/PPSSPP_1.13.1-18+infra_win.rar/file

First Im using wireshark (not master version because filters doesn't work) with the game on "localhost" to find and trigger informations from client (game) to -> server

Then I spotted differents things that the client (game) tried to do via the debugger in order ;

1. game tried to make several DNS check with the previous stun Server : mpostunus.konamionline.com (doesn't exist since May 2012)
2. Then tried to find the page with "terms of use" that you had to accept at : http://info.service.konamionline.com/VP029-U1/info/ (doesn't exist since May 2012)
3. It will tried to connect to "HTTPS" to find accounts, user names, password, games settings, etc.. at : https://mpoweb.konamionline.com/us/mpo/ (doesn't exist since May 2012) (Need to affiliate it to the IP of actual server and rewrite the "HTTP" URL via cheats that are already in the PPSSPP infra build above and redirected to http://savemgo.com/us/mpo/)
5. Then it will set you up to a "Server Lobby" on NA US version we have "gate02", Jap it's "gate01", EU is "gate03" at : mpogate02.konamionline.com (doesn't exist since May 2012)
6. Normally after all of these steps, game/client will be connected to the server, certainly we are gonna need to do more with other pages after that (Ranking, join host, create host, etc...)

Some screens from the official servers from 2012 shot by me ages ago (sorry it's in french) 

This page, which is still accessible today, leads to a stun server check "mpostunus.konamionline.com", a DNS check which results in a UDP error (P518)

![2](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/14ae83c1-cfeb-4bc0-8f7a-938f7443028d)


Therms of use page that the client tries to read on http://info.service.konamionline.com/VP029-U1/info/ (there is one page for each language like MGO1)

![5](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/77cf5b69-5e1b-4219-9899-090ab8b12dbc)


Session account (Open, create, change passwords, etc...) where the game will reach them on the URL https://mpoweb.konamionline.com/us/mpo/ 

![6](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/133601d4-d5cb-4ab6-9748-28cf2c453d4c)


Then the game looks for the "gate" that I described above 

![11](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/12b29659-ad15-4447-8d2e-ec488946ff9b)


and after picking a Lobby server, there we are : 

![15](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/418f1e5b-bcf4-4810-a1de-d758e4f7b2b4)

With different pages like join, create host, ranking etc...


Ranking looked like that : 

![16](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/850cd04b-1d7f-4aa1-8970-907f3df01a11)


Then you could select one player to see the personal ranking page :

![17](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/aeb75264-9b50-48a7-9212-a191e4199e9d)
![18](https://github.com/snakeswiss/Project-saveMPO-/assets/140389050/21f019bb-b25c-4b33-9ab7-c2ba948ed086)


Everything is strongly similar to MGO1 system Network Protocol that I use as a reference made by Zi (thank you very much for that !), since i'ts the same "architecture" except for DNAS check part that doesn't seems to exist in MPO.

Digital Network Authentication System : DNAS was a proprietary online authentication and anti-piracy system developed by Sony Computer Entertainment Inc. (SCEI) for use with PlayStation 2 and PlayStation Portable (PSP) games. It was designed to protect against unauthorized gameplay, cheating, and hacking in online multiplayer games. DNAS worked by verifying the legitimacy of the game disc and user account before allowing access to online features.

It was certainly very annoying to get it on some PS2 games, on PSP system I think that it was only used for downloading games/contents from PSN.

https://savemgo.com/
