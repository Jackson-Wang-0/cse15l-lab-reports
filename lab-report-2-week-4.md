# **Lab Report 2 - Week 4**
### _By: Zhicheng Wang, Pid: A16869487_

![58b180bcba5a92d7d95c58153c9ce5b2](https://user-images.githubusercontent.com/97211608/151492971-df483ed3-2d93-4421-a578-2a8e64d8eb46.png)

# **First Code Change**

## Code Change Difference From Github
<img align="right" width="1255" alt="截屏2022-01-27 下午10 00 44" src="https://user-images.githubusercontent.com/97211608/151495399-4df07f75-1061-4aad-bfa9-961a9060ecae.png">

## Link To The Test File
- [Click Me!!!](https://github.com/Jackson-Wang-0/cse15l-lab-reports/blob/main/test-file-new.md)

## Symptom of Failure-inducing Input
<img width="646" alt="截屏2022-01-27 下午10 18 17" src="https://user-images.githubusercontent.com/97211608/151497395-2eff180e-6d6a-42ab-ba40-9149c796292d.png">

- The symptom was that it was producing wrong outputs. Instead of **"only"** printing out the links of the file, it also printed out the image link. 

- This happens due to a bug in our code where whenever we see the following sequence in a file. We tend to store whatever is between the paranthesis into our array.
```
[]()
```

- **We can fix this bug by realizing that image always comes with an exclamation mark `!`** 

_Therefore, we add the if condition_

```
if (!(markdown.charAt(nextOpenBracket-1) == '!')) {
                 toReturn.add(markdown.substring(openParen + 1, closeParen));
             }
```
Where we would only store a link if it's open bracket doesn't come with an exclamation mark `!` before it, and that would fix the bug!


# **Second Code Change**

## Code Change Difference From Github
<img width="1225" alt="截屏2022-01-27 下午10 46 13" src="https://user-images.githubusercontent.com/97211608/151500514-f1662a6c-bae7-472a-9b8b-aea9d8822249.png">

## Link To The Test File
- [Click Me Again!!!](https://github.com/Jackson-Wang-0/cse15l-lab-reports/blob/main/test-file7.md)

## Symptom of Failure-inducing Input
<img width="630" alt="截屏2022-01-27 下午10 58 43" src="https://user-images.githubusercontent.com/97211608/151501858-4612397c-cf66-4a8d-a65a-56420b332cb0.png">

- The symptom was that our program keeps on looping and never stops which will end up with an out of memory error.

- The bug was caused by the file having the `)` at index 0 which will not update our `currentIndex` variable and result in an infinite loop

# **Last Code Change**

