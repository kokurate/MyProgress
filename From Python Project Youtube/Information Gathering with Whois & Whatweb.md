## [Back](https://github.com/kokurate/MyProgress/blob/main/From%20Python%20Project%20Youtube/introduction.md)


# Information Gathering

## Whois
## Simple Command 
```
whois dpr.go.id

```
![image](https://user-images.githubusercontent.com/85746411/217159090-7a4970fa-5b2e-49b7-9114-5c46cc046e23.png)

it will showed the several information


## Whatweb
### Very Simple Command
```
whatweb instagram.com
```

### To make this even more structured using verbose option (extension & plugin info justlike info.php)
```
whatweb instagram.com -v
```
This result can be scanning for vulnerability (IP Range)
```
Netmask (Network & Host)
Class A 255.0.0.0
Class B 255.255.0.0
Class C 255.255.255.0

** Note 255 = fixed
         0 = change
```

### How to scan the IP Range Vulnerability using whatweb ???

1. Find the IP Address just we did before
```
whatweb instagram.com -v
```

2. Then we can Scanning the IP Range
   For example the IP found is : 31.13.95.72
```
whatweb 31.13.95.0-31.13.95.255 -v

Note :  Status would be found if exist
        Red = error (not active)
```

### We can also save the scanning result to our local storage
1. Find the location you want to save

2. Using this syntax
```
whatweb instagram.com -v --log-verbose= {FILENAME}

ex. whatweb instagram.com -v --log-verbose=ifinfo
```

3. It will automatically saved in your local storage



