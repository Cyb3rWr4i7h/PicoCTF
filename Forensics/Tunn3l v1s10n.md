# tunn3l v1s10n
[Link](https://play.picoctf.org/practice/challenge/112?category=4&page=1) for this challenge.
Points: 40

## Solution
First I tried to see the filetype using `file` command but it didn't tell much so I used `xxd` tool to print the file headers
```bash
xxd tunn3l_v1s1on | head
```
(`head` command will print only the first 10 lines. I used it since I only need to see the file headers which are present in the first line)
This gave the output:
![File Headers](Images/tunnel1.png)

Here, the file headers looked like that of a `BMP` file. So I did a google search and then I stumbled upon [this](https://www.photopea.com) website which could display such files.
When I uploaded this file, I received:
![tunnel2](Images/tunnel2.png)




## Flag
picoCTF{qu1t3_a_v13w_2020}
