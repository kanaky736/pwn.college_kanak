# Challenge Name
an epic filesystem quest
## My solve
**Flag:** `pwn.college{MCkB2W5rtn9wN_900Y-7Gs4Ty75.QX5IDO0wSOyEzNzEzW}`

```bash
Connected!
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
SPOILER  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin      challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat SPOILER
Great sleuthing!
The next clue is in: /usr/share/javascript/mathjax/jax/output/SVG/fonts/Gyre-Termes/Size5
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/share/javascript/mathjax/jax/output/SVG/fonts/Gyre-Termes/Size5
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/SVG/fonts/Gyre-Termes/Size5$ ls
ALERT  Regular
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/SVG/fonts/Gyre-Termes/Size5$ cat ALERT
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/networkx/algorithms/isomorphism

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/SVG/fonts/Gyre-Termes/Size5$ ls /usr/lib/python3/dist-packages/networkx/algorithms/isomorphism
WHISPER-TRAPPED  __pycache__  isomorph.py     matchhelpers.py         tests
__init__.py      ismags.py    isomorphvf2.py  temporalisomorphvf2.py  vf2userfunc.py
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/SVG/fonts/Gyre-Termes/Size5$ cat /usr/lib/python3/dist-packages/networkx/algorithms/isomorphism/WHISPER-TRAPPED
Congratulations, you found the clue!
The next clue is in: /opt/pwndbg/.venv/lib/python3.8/site-packages/pynacl-1.6.0.dist-info/licenses

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/SVG/fonts/Gyre-Termes/Size5$ cd /opt/pwndbg/.venv/lib/python3.8/site-packages/pynacl-1.6.0.dist-info/licenses
hacker@commands~an-epic-filesystem-quest:/opt/pwndbg/.venv/lib/python3.8/site-packages/pynacl-1.6.0.dist-info/licenses$ ls -a
.  ..  .HINT  LICENSE
hacker@commands~an-epic-filesystem-quest:/opt/pwndbg/.venv/lib/python3.8/site-packages/pynacl-1.6.0.dist-info/licenses$ cat .HINT
Lucky listing!
The next clue is in: /usr/share/icons/hicolor/72x72/animations

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/pwndbg/.venv/lib/python3.8/site-packages/pynacl-1.6.0.dist-info/licenses$ cd /usr/share/icons/hicolor/72x72/animations
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/72x72/animations$ ls
LEAD
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/72x72/animations$ cat LEAD
Tubular find!
The next clue is in: /usr/lib/python3/dist-packages/tornado-5.1.1.egg-info
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/72x72/animations$ cd /usr/lib/python3/dist-packages/tornado-5.1.1.egg-info
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/tornado-5.1.1.egg-info$ ls
CUE  PKG-INFO  dependency_links.txt  top_level.txt
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/tornado-5.1.1.egg-info$ cat CUE
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/mistune-0.8.4.egg-info
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/tornado-5.1.1.egg-info$ cd /usr/lib/python3/dist-packages/mistune-0.8.4.egg-info
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/mistune-0.8.4.egg-info$ ls
GIST  PKG-INFO  dependency_links.txt  not-zip-safe  top_level.txt
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/mistune-0.8.4.egg-info$ cat GIST
Tubular find!
The next clue is in: /opt/linux/linux-5.4/arch/arm64/boot/dts/ti

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/mistune-0.8.4.egg-info$ cd /opt/linux/linux-5.4/arch/arm64/boot/dts/ti
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm64/boot/dts/ti$ ls -a
.      Makefile           k3-am65-wakeup.dtsi      k3-am654.dtsi                   k3-j721e-mcu-wakeup.dtsi
..     k3-am65-main.dtsi  k3-am65.dtsi             k3-j721e-common-proc-board.dts  k3-j721e-som-p0.dtsi
.NOTE  k3-am65-mcu.dtsi   k3-am654-base-board.dts  k3-j721e-main.dtsi              k3-j721e.dtsi
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm64/boot/dts/ti$ cat .NOTE
Congratulations, you found the clue!
The next clue is in: /usr/local/lib/python3.8/dist-packages/pyelftools-0.32.dist-info

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm64/boot/dts/ti$ ls /usr/local/lib/python3.8/dist-packages/pyelftools-0.32.dist-info
INSTALLER  LICENSE  METADATA  RECORD  TIP-TRAPPED  WHEEL  top_level.txt
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/arm64/boot/dts/ti$ cat /usr/local/lib/python3.8/dist-packages/pyelftools-0.32.dist-info/TIP-TRAPPED
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{MCkB2W5rtn9wN_900Y-7Gs4Ty75.QX5IDO0wSOyEzNzEzW}
```
## Incorrect tangents I went on
none

## What I learned
I learned how to use cat, cd, ls functions efficiently 
## References 
none

