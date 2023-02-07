## [back](https://github.com/kokurate/MyProgress/blob/main/From%20Python%20Project%20Youtube/introduction.md)

# Creating IP Checker using python (Tool)

1. Using nano as a text editor in terminal
```
nano checkip.py
```

2. Here's the code
```
import socket

hostname = input('Enter a domain name: ')
ip_address = socket.gethostbyname(hostname)

print(f'Domain Name: {hostname}')
print(f'IP Address : {ip_address}')

```

3. Then run the command using
```
python checkip.py 
```
enter the domain name and it will show the ip address of the domain name

![image](https://user-images.githubusercontent.com/85746411/217155667-82244b05-b391-4341-9419-e187c265c26a.png)

4. Then we compare to
```
nslookup
```
![image](https://user-images.githubusercontent.com/85746411/217155863-f89c4632-50cf-4bf5-a3d9-8acd97f011b0.png)

and it will be the same
