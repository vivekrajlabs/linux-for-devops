# Setup: get a free Linux machine

Every lab is tested on **Ubuntu 24.04 LTS**. Pick one option.

## Windows: WSL (recommended)

1. Open **PowerShell as Administrator**.
2. Run:
   ```powershell
   wsl --install
   ```
3. Restart when asked, then open **Ubuntu** from the Start menu and create a username and password.

## Mac: Multipass

1. Install Homebrew if you don't have it: https://brew.sh
2. Then:
   ```bash
   brew install multipass
   multipass launch 24.04 --name devops
   multipass shell devops
   ```
   You are now inside a real Ubuntu machine. Type `exit` to leave; `multipass shell devops` to come back.

## Any computer: a free cloud VM

Create an Ubuntu 24.04 instance on the free tier of AWS, Google Cloud, Azure or Oracle Cloud, and connect with SSH
(Episode 17 covers SSH in detail). Remember to **stop or delete** it when you're done so you're never billed.

## Check it worked

```bash
lsb_release -d
```

You should see something like `Description:	Ubuntu 24.04.1 LTS`. You're ready for [Episode 1](ep01-what-is-linux/).
