> Zipfil

Here the zipfile seems to be broken. So I checked the hex of the zipfile. First I tried to change magic bytes to that of zip file but failed. So after asking hints around I observed the zip file magic header in reverse order. Looks like the hex is inverted. So I inverted them manually and `cat $file | xxd -r -p > file.zip`.

Now the zip is password potected. So I used john!

```bash
zip2john file.zip > hash
john hash --wordlist=/usr/share/wordlists/rockyou.txt
123456           (file.zip/flag.txt)
```

# Flag

```
StormCTF{Misc2:B73dba52ceDA4dDccb31Ec1b1cDa24Ff}
```