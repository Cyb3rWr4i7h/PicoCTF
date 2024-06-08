# MSB
[Link](https://play.picoctf.org/practice/challenge/359?category=4&page=3) for this challenge
Points: 200

## Solutions
The name of the challenge suggests that it might have something to do with the Most Significant Bit of pixels of given image. To extract the data from the MSB, a found a python tool called [sigBits](https://github.com/Pulho/sigBits): A Steganography significant bits image decoder. It required a library `pillow` so I downloaded it using 
```bash
pip install pillow
```
