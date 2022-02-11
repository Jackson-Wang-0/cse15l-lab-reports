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

- Notice that there were a lot of "extra" stuff that you don't recognize, it is also copying the hidden files when making commits so it will take a long time.


## Compiling and Running the tests in ieng6 account 

<img width="664" alt="截屏2022-02-11 上午12 54 59" src="https://user-images.githubusercontent.com/97211608/153562772-8a1f8f96-7edb-4c54-ac0c-db06b2b02f19.png">

- After logging into the ieng6 account and using the `ls markdown-parse` command, we can see that all the files have been copied over, even the ones we would see in `.git`

_Then after `cd` into `markdown-parse`_

- We can now compile and run the tests for our repository !

<img width="820" alt="截屏2022-02-11 上午1 06 49" src="https://user-images.githubusercontent.com/97211608/153564168-596569c4-8b25-4da7-a10d-e439dfc07e7c.png">

- All 8 tests passed with no errors :)

## combining `scp`, `;`, and `ssh` to copy the whole directory and run the tests in one line

 ```
$ scp -r . cs15lwi22awg@ieng6.ucsd.edu:~/markdown-parse; javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java; java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest

 ```
