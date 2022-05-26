

# Windows icin Choco uzerinden kubectl kurulum:

- https://chocolatey.org/install

- Chocolatey Windows paket yoneticisidir.

### Chocolatey Kurulum

- Ilk once PowerShell i Administrator olarak calistiririz:

```bash

 $ Set-ExecutionPolicy AllSigned

 $ Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol \
 = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient) \
 .DownloadString('https://community.chocolatey.org/install.ps1'))

```

- Ardından bu komut ile yuklemis oluruz <-- Chocolatey
```bash
 $ choco -?
```
- Bu komut ile kontrol edilir.

### Choco ile kubectl kurulum
```bash
 $ choco install kubernetes-cli

 $ kubectl version
```
- Komutu ile kubectl yukleme durunu kontrol eder.

# Mac ve Linux kubectl kurulum:

### Brew ile kubectl kurulum

- Brew Mac ve Linux'un paket yoneticisidir.

- https://brew.sh

```bash

 $ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

```

- Terminale yapıstırılır ve duruma baglı olarak root sifresi sorabilir.
```bash
 $ brew  <-- komutu ile kontrol edilir.
```
## kubectl

```bash
 $ brew install kubectl

 $ kubectl version
```

- Komutu ile yuklendigini gormus oluruz.