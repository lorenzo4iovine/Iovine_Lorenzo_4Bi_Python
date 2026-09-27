# Autenticazione verso GitHub

## Metodo Scelto
Ho scelto l'autenticazione tramite chiave SSH.

@lorenzo4iovine ➜ /workspaces/Iovine_Lorenzo_4Bi_Python (main) $ ssh-keygen -t ed25519 -C "lorenzo.iovine@marconirovereto.it"
Generating public/private ed25519 key pair.
Enter file in which to save the key (/home/codespace/.ssh/id_ed25519): 
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/codespace/.ssh/id_ed25519
Your public key has been saved in /home/codespace/.ssh/id_ed25519.pub
The key fingerprint is:
SHA256:/Rm2r8hrqbTcJmWP5sRVW8evspgqTnfQzA9a2SRApiI lorenzo.iovine@marconirovereto.it
The key's randomart image is:
+--[ED25519 256]--+
|       .+        |
|       o .     . |
|  E . .   . . . +|
|   . .   = = . oo|
|        S O = . .|
|         =o* + . |
|      . +o++* .  |
|     ..+.**+.+   |
|     ...=OO.o..  |
+----[SHA256]-----+
@lorenzo4iovine ➜ /workspaces/Iovine_Lorenzo_4Bi_Python (main) $ cat ~/.ssh/id_ed25519.pub
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIMpbL0OARnpmFN1RRlQvZaKQr3jDjdrw+fznTSVaPJKH lorenzo.iovine@marconirovereto.it