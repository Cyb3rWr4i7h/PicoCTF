# Mod 26
[Link](https://play.picoctf.org/practice/challenge/144?category=2&page=1) for this challenge

Points: 10

## Writeup
The challenge mentions `ROT 13` in the desciption along with the text `cvpbPGS{arkg_gvzr_V'yy_gel_2_ebhaqf_bs_ebg13_MAZyqFQj}` so I rotated the text by 13 using `tr` tool:
```bash
echo "cvpbPGS{arkg_gvzr_V'yy_gel_2_ebhaqf_bs_ebg13_MAZyqFQj}" | tr 'A-Za-z' 'N-ZA-Mn-za-m'\n
```

This gave the flag

## Flag
picoCTF{next_time_I'll_try_2_rounds_of_rot13_ZNMldSDw}

## Extra
- To know about `ROT 13`, check [this](https://en.wikipedia.org/wiki/ROT13) wikipedia page
- To know `tr` tool, check out [this](https://www.man7.org/linux/man-pages/man1/tr.1.html) manpage or simply run `man tr` in linux terminal
