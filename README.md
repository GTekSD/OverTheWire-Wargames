```
      ,----..            ,----,          .---.
     /   /   \         ,/   .`|         /. ./|
    /   .     :      ,`   .'  :     .--'.  ' ;
   .   /   ;.  \   ;    ;     /    /__./ \ : |
  .   ;   /  ` ; .'___,/    ,' .--'.  '   \' .
  ;   |  ; \ ; | |    :     | /___/ \ |    ' '
  |   :  | ; | ' ;    |.';  ; ;   \  \;      :
  .   |  ' ' ' : `----'  |  |  \   ;  `      |
  '   ;  \; /  |     '   :  ;   .   \    .\  ;
   \   \  ',  /      |   |  '    \   \   ' \ |
    ;   :    /       '   :  |     :   '  |--"
     \   \ .'        ;   |.'       \   \ ;
  www. `---` ver     '---' he       '---" ire.org
```
# Welcome to OverTheWire!

### Wargames : All Level Walkthroughs

1. [Bandit](Bandit.md)
2. [Natas](Natas.md)
3. [Leviathan](Leviathan.md)
4. [Krypton](Krypton.md)
5. [Narnia](Narnia.md)
6. [Behemoth](Behemoth.md)
7. [Utumno](Utumno.md)
8. [Maze](Maze.md)
9. [Vortex](Vortex.md)
10. [Manpage](Manpage.md)
11. [Drifter](Drifter.md)
12. [FormulaOne](FormulaOne.md)

_If you find any problems, please report them to the #wargames channel on discord or IRC._

### --[ Playing the games ]--

This machine might hold several wargames.
If you are playing "somegame", then:

* USERNAMES are somegame0, somegame1, ...
* Most LEVELS are stored in /somegame/.
* PASSWORDS for each level are stored in /etc/somegame_pass/.


_Write-access to homedirectories is disabled. It is advised to create a working directory with a hard-to-guess name in /tmp/.  You can use the command "mktemp -d" in order to generate a random and hard to guess directory in /tmp/.  Read-access to both /tmp/ is disabled and to /proc restricted so that users cannot snoop on eachother. Files and directories with easily guessable or short names will be periodically deleted! The /tmp directory is regularly wiped._

**Please play nice:**

* don't leave orphan processes running
* don't leave exploit-files laying around
* don't annoy other players
* don't post passwords or spoilers
* again, DONT POST SPOILERS!

This includes writeups of your solution on your blog or website!

### --[ Tips ]--

This machine has a 64bit processor and many security-features enabled by default, although ASLR has been switched off.  The following compiler flags might be interesting:

    -m32                    compile for 32bit
    -fno-stack-protector    disable ProPolice
    -Wl,-z,norelro          disable relro

  In addition, the execstack tool can be used to flag the stack as
  executable on ELF binaries.

  Finally, network-access is limited for most levels by a local
  firewall.

### --[ Tools ]--

 For your convenience we have installed a few useful tools which you can find
 in the following locations:

* gef (https://github.com/hugsy/gef) in /opt/gef/
* pwndbg (https://github.com/pwndbg/pwndbg) in /opt/pwndbg/
* peda (https://github.com/longld/peda.git) in /opt/peda/
* gdbinit (https://github.com/gdbinit/Gdbinit) in /opt/gdbinit/
* pwntools (https://github.com/Gallopsled/pwntools)
* radare2 (http://www.radare.org/)

Both python2 and python3 are installed.

### --[ More information ]--

For more information regarding individual wargames, visit http://www.overthewire.org/wargames/

For support, questions or comments, contact us on discord or IRC.

Enjoy your stay!
