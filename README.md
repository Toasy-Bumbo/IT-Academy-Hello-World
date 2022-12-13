# IT-Academy-Hello-World
First repository
1. Inleiding

3. Hoofdstuk 1 Wat is dit?

Dit is een MarkDown file waarin interresante informatie over dit project staat.

3. Hoofdstuk 2 Hyperinks gebruiken

[Beste zoekmachine](https://duckduckgo.com)

4. SSH sleutel maken

ssh-keygen -t ed25519 -C "test@domain.com"

Gebruik hierbij je eigen e-mail addres waarmee je in Github inlogd

Kopieer de publieke sleutel uit de ~/.ssh directory uit het bestand met de naam zoals in de stappen hierboven is aangegeven (C:\Users\<USERNAME>\.ssh\id_rsa.pub).
Let erop om de publieke en niet de private sleutel (C:\Users\<USERNAME>\.ssh\id_rsa)te kopieren . Kopieer de publieke sleutel in Gitlab/GitHub
IN GitHub, ga naar je profile, klik op settings en ga naar SSH- GPY key.
Klik "New SSH key"

Nu kan je inloggen zonder usename password

C:\windows\system32>ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (C:\Users\<USERNAME>/.ssh/id_rsa):
Created directory 'C:\Users\<USERNAME>/.ssh'.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in C:\Users\<USERNAME>/.ssh/id_r<USERNAME>/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:******************************************* <USERNAME>@<COMPUTERNAME>
The key's randomart image is:
+---[RSA 3072]----+
|     +=*=o  ..   |
|     .+=B o.  .  |
|    . .+.*.  o   |
|     **********  |
|    o . So.E   . |
|       o oo o +  |
|        o .. = + |
|         o  ..* o|
|            *****|
+----[SHA256]-----+

C:\windows\system32>


5. Git installeren

https://git-scm.com/download/win
winget install --id Git.Git -e --source winget

