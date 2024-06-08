# MSB
[Link](https://play.picoctf.org/practice/challenge/359?category=4&page=3) for this challenge
Points: 200

## Solution
The name of the challenge suggests that it might have something to do with the Most Significant Bit of pixels of given image. To extract the data from the MSB, a found a python tool called [sigBits](https://github.com/Pulho/sigBits): A Steganography significant bits image decoder. It required a library `pillow` so I downloaded it using 
```bash
pip install pillow
```
Then I downloaded the `sigBits.py` script using:
```bash
wget https://raw.githubusercontent.com/Pulho/sigBits/master/sigBits.py
```
or one can create using text editor and paste [this](https://github.com/Pulho/sigBits/blob/master/sigBits.py) script

Then I simply ran `sigBits.py` script with `-t` option set to msb:
```bash
python3 sigBits.py -t=msb Ninja-and-Prince-Genji-Ukiyoe-Utagawa-Kunisada.flag.png
```
Then I searched for the flag in the file created (`outputSB.txt`) by opening it with vim text editor and seaching using `/pico`
```bash
vim outputSB.txt
```
And then searchin
## Flag
picoCTF{15_y0ur_que57_qu1x071c_0r_h3r01c_24d55bee}
