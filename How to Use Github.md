# How to Use Github

## Download Git:  [`link`](https://git-scm.com/download)
- check version: `git --version`
- if it return with `git version x.xx.x`, configuration successed.

## Initialization
- configure email & user
```java
git config --global user.name "IceCoffee98"
git config --global user.email "yixuanyu98@gmail.com"
```
- check your configuration
```java
git config --list
```

## Local Management
### Set Git Repository
```java
cd /Users/jesse/Documents/git_test // go into the fold
ls // list all files existing in this fold
pwd // show current directory
```
<img src="/Users/jesse/Library/Application Support/typora-user-images/image-20200330002806856.png" alt="image-20200330002806856" style="zoom:50%;" align='left' />
```java
mkdir test1 // creat dir 
cd test1 // go into the fold just created before
git init // set repository
```
<img src="/Users/jesse/Library/Application Support/typora-user-images/image-20200330003851824.png" alt="image-20200330003851824" style="zoom:50%;" align='left' />

### Add Files into the Repository
```java
git status //check the status of this repository
```
<img src="/Users/jesse/Library/Application Support/typora-user-images/image-20200330004627509.png" alt="image-20200330004627509" style="zoom:50%; align='left'" />

```java
touch a1.php // creat a new file named 'a1.php'
git status
```
![image-20200330004804443](/Users/jesse/Library/Application Support/typora-user-images/image-20200330004804443.png)

### Add to Staging Area
```java
git add a1.php
git status
```
![image-20200330005009193](/Users/jesse/Library/Application Support/typora-user-images/image-20200330005009193.png)

### Commit to Respository
```java
git commit -m 'first time added'
git status
```
![image-20200330005533309](/Users/jesse/Library/Application Support/typora-user-images/image-20200330005533309.png)

### Revise Files in Respository
```java
vi a1.php //edit a1.php by vim
cat a1.php
git status
git add a1.php
git status
git commit  -m 'add my first revised a1.php to repository'
```
![image-20200330010912874](/Users/jesse/Library/Application Support/typora-user-images/image-20200330010912874.png)

![image-20200330011626646](/Users/jesse/Library/Application Support/typora-user-images/image-20200330011626646.png)

### Deletes Files in Respository
```java
rm a1.php
git rm a1.php
git commit -m 'my first deleted file'
```
![image-20200330012203273](/Users/jesse/Library/Application Support/typora-user-images/image-20200330012203273.png)



## Remote Management

- the first 3 steps are the same as that in local management, but you need add  `git push` in the end to push the repository into github.

![image-20200330015635487](/Users/jesse/Library/Application Support/typora-user-images/image-20200330015635487.png)

