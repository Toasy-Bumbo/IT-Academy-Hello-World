# IT-Academy-Hello-World
First repository
1. _**Inleiding**_

Niets te melden...

3. **Hoofdstuk 1 Wat is dit?**

Dit is een MarkDown file waarin interresante informatie over dit project staat.

3. **Hoofdstuk 2 Hyperinks gebruiken**

[Beste zoekmachine](https://duckduckgo.com)

4. **SSH sleutel maken**

ssh-keygen -t ed25519 -C "test@domain.com"

(-t is de codering. Kan ook alleen ssh-keygen <enter> op de commandline en alleen mailadres opgeven, dan wordt een andere codering gebruikt) 

Gebruik hierbij je eigen e-mail addres waarmee je in Github inlogd.

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



5. **Username en e-mail toevoegen aan GitConbfig**

      C:\Users\Mathijs\Python\Hello World>git config --global user.name Toasy-Bumbo

      C:\Users\Mathijs\Python\Hello World>git config --global user.email m.w.hagenaar@kpnplanet.nl

      C:\Users\Mathijs\Python\Hello World>git config --list
      diff.astextplain.textconv=astextplain
      filter.lfs.clean=git-lfs clean -- %f
      filter.lfs.smudge=git-lfs smudge -- %f
      filter.lfs.process=git-lfs filter-process
      filter.lfs.required=true
      http.sslbackend=openssl
      http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
      core.autocrlf=true
      core.fscache=true
      core.symlinks=false
      pull.rebase=false
      credential.helper=manager
      credential.https://dev.azure.com.usehttppath=true
      init.defaultbranch=master
      user.name=<Git username>
      user.email=<test>@domain.com
      
6. **Git installeren**

  [git download site](https://git-scm.com/download/win)

  winget install --id Git.Git -e --source winget
  
  Ga naar de repository, klik op de groene knop 'Code' en klik op het tabblad SSH. Kopieer de link.
  
  Maak in de user directory een lege directory aan. Start een command shell en ga naar de lege directoryc.
  
          C:\Users\Mathijs\Python\Hello World>git clone git@github.com:Toasy-Bumbo/IT-Academy-Hello-World.git
          Cloning into 'IT-Academy-Hello-World'...
          The authenticity of host 'github.com (140.82.121.3)' can't be established.
          ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
          This key is not known by any other names.
          Are you sure you want to continue connecting (yes/no/[fingerprint])? y
          Please type 'yes', 'no' or the fingerprint: yes
          Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
          remote: Enumerating objects: 30, done.
          remote: Counting objects: 100% (30/30), done.
          remote: Compressing objects: 100% (19/19), done.
          remote: Total 30 (delta 8), reused 0 (delta 0), pack-reused 0
          Receiving objects: 100% (30/30), 7.16 KiB | 2.39 MiB/s, done.
          Resolving deltas: 100% (8/8), done.

          C:\Users\Mathijs\Python\Hello World>
      
      Nu staat de Git clone op je computer.
      
  6. **Wat heb je nu?**
      
      Er is een working dorectory = Hier staan je bestanden
      Index = een buffer zone
      HEAD = verwijst naar je laatst gemaakte commit
      
      In Visual studio COde -> Open Folder (Folder waarin je Git Clone op hebt uitgevoerd)
      
      Maak nun een wijziging in readme.md aan en het wijzigd nu ook in GitHub ;)
      
      _Dit is een wijziging vanuit Visual Code_
      _Deze wijziging kan je vanuit Visual COde naar Github dorvoeren door in Visual Code op het commit icoon (twee pijltjes in een cirkel) linksonder in het scherm te klikken!_ 
      
  
  

