> Shark Fail

We have an interesting capture! I thought!

Run strings in the file and got a long string at the end. Let's put it in cyberchef!

```bash
strings sharkfail.pcapng | tail -n 26

U3Rvcm1DVEZ7TWlzYzI6NzZlRjEyNDE2Mzc2M0IzNTJCOTg4Y0JBMWU3NzVBOEF9
USBSK
USBCL
DALI       
OR1        
TRASHE~1   
OR1        
OOKMA~1HTM 
OUVEA~1   
_~1     TRA"
NNEXE~1PDF 
USBSL
USBCM
USBSM
USBCN
USBSN
USBCO
USBSO
Counters provided by dumpcap
3aM{
Counters provided by dumpcap
3aM{
Counters provided by dumpcap
3aM{
Counters provided by dumpcap
3aM{
```
Looks like b64 encoded!

echo U3Rvcm1DVEZ7TWlzYzI6NzZlRjEyNDE2Mzc2M0IzNTJCOTg4Y0JBMWU3NzVBOEF9 | base64 -d

```
StormCTF{Misc2:76eF124163763B352B988cBA1e775A8A}
```
