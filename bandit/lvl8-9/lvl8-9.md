# Goal 
The password for the next level is stored in the file data.txt and is the only line of text that occurs only once
# Step
So in this lvl I will use command `uniq`, to make sure it will work use `sort` instead of `cat`
```bash 
snort data.txt | uniq -u
```
# Password
```bash 
EjmOSvuAu7sGAHqHVcBDPirRe9T03kxl
```
As we can see
 ![output](output.png)