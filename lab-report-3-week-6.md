# **Lab Report 3 - Week 6**
### _By: Zhicheng Wang, Pid: A16869487_

![1644386274583542](https://user-images.githubusercontent.com/97211608/153555814-bc088786-6921-431d-9690-c4838356807a.jpg)

# **Copy whole directories with `scp -r`**

## Copying markdown-parse Directory to ieng6 account

- Run the following command

```
scp -r . cs15lwi22@ieng6.ucsd.edu:~/markdown-parse
```

<img width="831" alt="截屏2022-02-11 上午12 08 49" src="https://user-images.githubusercontent.com/97211608/153557008-767000eb-1f8d-40dc-97b0-a7d907b31b23.png">

- The above is just part of the process when copying the whole directory ! 
- Notice that there were a lot of "extra" files that you don't recognize, it is also copying the hidden files when making commits so it will take a long time.
