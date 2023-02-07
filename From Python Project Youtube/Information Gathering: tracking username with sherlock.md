### [Back](https://github.com/kokurate/MyProgress/blob/main/From%20Python%20Project%20Youtube/introduction.md)

# Information Gathering Tracking Username
we can track social media accounts with username using sherlock

## sherlock

For more information just visit the official documentation right here : https://github.com/sherlock-project/sherlock 

### installing the sherlock
```
git clone https://github.com/sherlock-project/sherlock 
```

### installing the requirements
Before we can use sherlock, first we have to install all the requirements. To check this requirements you can follow this step :
1. go to the sherlock directory, i assuming that you are in the same directory with sharelock, so you can use
```
cd sherlock/
```
2. You can check all the requirements
```
cat requirements.txt 
```
3. Install the requirements 
Before you run this code, make sure you are already in the sherlock directory
```
python -m pip install -r requirements.txt
```

### Tracking the username
1. Go to directory /sherlock/sherlock
2. run the sherlock.py
```
python sherlock.py
```

maybe we can use username from email address that we tracking before (ex. hunter.io) 
3. If we got the username, next we can go to finding the social media accounts
make sure you already in directory sherlock/sherlock
```
python sherlock.py {username} {option}
```
4. We must use several options to make sure our searching is working properly
using timeout we will avoid websites with slow response
```
python sherlock.py {username} --timeout 5
```

5. Option Print all to see what websites sherlock has scanned to find the kokurate username and apparently there is no kokurate username on the website
```
python sherlock.py kokurate --timeout 5 --print-all
```

6. We can save the result to our local storage 
by adding output options
```
python sherlock.py kokurate --timeout 5 --print-all --output ~/Desktop/sharelock_result
```
![image](https://user-images.githubusercontent.com/85746411/217250901-e83adacf-117f-4ead-a8ea-632a4f5a89f5.png)

7. You can now see the file by using 
```
cat
```


