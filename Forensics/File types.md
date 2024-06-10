# File types
[Link](https://play.picoctf.org/practice/challenge/268?category=4&page=2) for this challenge

Points: 100

## Writeup
First I checked the filetype using `file` tool:
```bash
file Flag.pdf
```

![File1](Images/File1.png)

Since it's shell achive text, I tried to execute it which gave:

![File2](Images/File2.png)

This indicated that `uudecode` utility was not present so I downloaded it using:
```bash
sudo apt install sharutils
```
Then I tried to execute `Flag.pdf` again which gave:

![File3](Images/File3.png)

So I checked the directory for any new files and found a new file called `flag`. Then I checked its filetype.

![File4](Images/File4.png)

Since it's a `current ar archive` I changed its extension to `.ar`. Then I checked it's filetype again:

![File5](Images/File5.png)

