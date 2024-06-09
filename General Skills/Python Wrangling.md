# Python Wrangling
[Link](https://play.picoctf.org/practice/challenge/166?category=5&page=1) for this challenge

Points: 10

## Writeup
As clear from the file names; `flag.txt.en` contains the encrypted password, `ende.py` contains the python script and `pw.txt` contains the password.
In `ende.py` script, I saw this part:
```python
lif sys.argv[1] == "-h" or sys.argv[1] == "--help":
    print(help_msg)
    sys.exit(1)
```
So I ran this script with `-h` argument:
```bash
python3 ende.py -h
```
This gave:

![Wrangling1](Wrangling1.png)

Since the file I needef to decrypt is flag.txt.en, I ran this command:
```bash
python3 ende.py -d flag.txt.en
```
When prompted for password, I entered the text from `pw.txt` file.

![Wrangling2](Wrangling2.png)

This gave the decrypted flag.

## Flag
picoCTF{4p0110_1n_7h3_h0us3_aa821c16}
