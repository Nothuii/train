# Goal 
The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size
# Step 
Run the command based on hints above
```bash
find -user bandit7 -group bandit6 -type f -size 33c
```
the system displays a lot of `Permission denied` errors. To filter out these errors redirect stderr to `2>dev/null`
```bash 
find -user bandit7 -group bandit6 -type f -size 33c 2>dev/null
```
Output
```bash 
/var/lib/dpkg/info/bandit7.password
```
Read the file content to get the password:
```bash 
cat /var/lib/dpkg/info/bandit7.password
```
# Password
```bash
Bmnnvf82KzQlfxgAI2d1zYbr1u9pr3E3
```