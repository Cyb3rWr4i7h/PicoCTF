# Forensics
![Link](https://play.picoctf.org/practice?category=4&page=1) for challenges

## Information
We can see the image's metadata using `exiftool` as:
```bash
exiftool cat.jpg
```
It gives: 
  ![Information](Images/Information.jpg)
Looking at its metadata, the `License` string looks different so I decoded it using        ![Cyberchef](cyberchef.org)
Since its base64 decoded, we can also decode it using
```bash
echo cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9 | basee64 -d
```
### Flag
picoCTF{the_m3tadata_1s_modified} 

