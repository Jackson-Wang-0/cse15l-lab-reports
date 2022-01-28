# **Lab Report 2 - Week 4**
### _By: Zhicheng Wang, Pid: A16869487_

![58b180bcba5a92d7d95c58153c9ce5b2](https://user-images.githubusercontent.com/97211608/151492971-df483ed3-2d93-4421-a578-2a8e64d8eb46.png)

# First Code Change 

## code change diff from Github
- <img align="right" width="1255" alt="截屏2022-01-27 下午10 00 44" src="https://user-images.githubusercontent.com/97211608/151495399-4df07f75-1061-4aad-bfa9-961a9060ecae.png">

## Link to the test file
- [Test File1](https://jackson-wang-0.github.io/test-file-new.html)

## Symptom of failure-inducing input
- <img width="646" alt="截屏2022-01-27 下午10 18 17" src="https://user-images.githubusercontent.com/97211608/151497395-2eff180e-6d6a-42ab-ba40-9149c796292d.png">

- The symtptom was that it was producing wrong outputs. Instead of **"only"** printing out the links of the file, it also printed out the image link. This happens due to a bug in our code where whenever we see the following sequence in a file (_open Bracket followed by closed Bracked and then followed by open and closed Paranthesis_). We tend to store whatever is between the paranthesis into our array.
```
[]()
```
- We can fix this bug by realizing that image always comes with an exclamation mark `!` 

Therefore, we add the if condition
```
if (!(markdown.charAt(nextOpenBracket-1) == '!')) {
                 toReturn.add(markdown.substring(openParen + 1, closeParen));
             }
```
We would only store a link if it's open bracket doesn't come with an exclamation mark `!` before it, and that would fix the bug!


# Second Code Change

# Last Code Change

