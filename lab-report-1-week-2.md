## Welcome to Zhicheng's first lab report!!!!

![https---specials-images forbesimg com-imageserve-617853670-Drive-by-hacker-960x0 jpg?fit=scale](https://user-images.githubusercontent.com/97211608/149288135-be00f80e-86a7-4427-b4b0-72a4bad9f2f5.jpeg)


### Let's begin the Tutorial !!!
# Visual Studio Code

1. First, You need to download [Visual Studio Code](https://code.visualstudio.com) on your computer. After it is installed, double click the icon and you will end up in a screen which looks something like this. (it could be a little different)

<img width="1024" alt="截屏2022-01-12 下午11 14 40" src="https://user-images.githubusercontent.com/97211608/149283051-fae79476-3c5c-4aff-bbd6-0204ace0fb86.png">

# Remotely Connecting

- Window users need to [install OpenSSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse) to connect your computer to another computer.

Next, each student have their own course-specific account which can be found at: [Account Lookup](https://sdacs.ucsd.edu/~icc/index.php)


_Note: for CSE15L, our account starts with **cs15lwi22**_


Enter the following command but replace `abc` with the letters of your course-specific account 


```
ssh cs15lwi22abc@ieng6.ucsd.edu
```

If this is your first time connecting to a server, you will get a message like this:
```
Are you sure you want to continue connecting (yes/no/[fingerprint])? 
```
We usually type `yes` in this case and then it will ask for your password!

After you successfully logged in with your password, the output should look like this：

<img width="686" alt="截屏2022-01-13 下午5 49 07" src="https://user-images.githubusercontent.com/97211608/149437544-1fce6089-df67-437d-8768-1875fbbbded7.png">

If you made it this far, congrats! Your terminal is now connected!!!

# Trying Some Commands

Below are some commands you can try on your own:

- `cd~`  navigate to your home directory
- `cd` navigate to your home directory
- `ls -lat` list latest files
- `ls -a` list all files
- `ls<directory>` where `<directory>` is `/home/linux/ieng6/cs15lwi22/cs15lwi22abc/`
- `cp /home/linux/ieng6/cs15lwi22/public/hello.txt ~/`
- `cat /home/linux/ieng6/cs15lwi22/public/hello.txt`

Logout command:

- `exit`

After typing in `exit` you should receive the following message:

<img width="471" alt="截屏2022-01-13 下午7 39 48" src="https://user-images.githubusercontent.com/97211608/149447606-315fce80-e936-490d-af7d-83fb30561b38.png">

# Moving Files with `scp`




You can use the [editor on GitHub](https://github.com/Jackson-Wang-0/Week-2-Lab-Report/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.


```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Jackson-Wang-0/Week-2-Lab-Report/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

cool
