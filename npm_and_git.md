# Install the necessary tools

We use NodeJS’s Package Manager to install the mist-CLI, so we first need to install the package manager. All code is managed with Git, which we also need to install.

## Install NodeJS

1. Go to [https://nodejs.org/en/](https://nodejs.org/en/) and download the LTS version.
2. Go through the installer.
3. Verify the installation by opening PowerShell (or another terminal) and running the command: 
   ```bash
   npm --version
   ```

   > ```bash
   > 8.18.0
   > ```

## Install Git

1. Go to [https://git-scm.com/downloads](https://git-scm.com/downloads), and download the installer.
2. Go through the installer.
3. Verify the installation by opening *git bash* and running the command: 
   ```bash
   git --version
   ```
   > ```bash
   > git version 2.37.3.windows.1
   > ```


> ⚠️ Because mist-cli interacts with Git, all mist-commands must be run in a terminal that can execute `git` commands. For windows users we recommend Git Bash.

## Set up SSH

All administrative commands are executed via a secure connection (SSH). Therefore we need to verify that we are connected directly to mist-cloud, with no one listening to the communication. To enforce this, add mist-cloud to the 'known hosts' with the command:

```bash
echo "api.mist-cloud.io ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIOW2dgo+0nuahOzHD7XVnSdrCwhkK9wMnAZyr6XOKotO" >> ~/.ssh/known_hosts
```

To verify the connection we need to set up a new user account.

