# Node Commands

## Prerequisites

Before using these commands, ensure that `nvm` is installed on your system. If `nvm` is not installed, you can follow the instructions on the [official nvm GitHub page](https://github.com/nvm-sh/nvm) to set it up.

## Commands

Below are the common `nvm` commands used to manage Node.js versions:

### Check the Current Node Version

```bash
node -v
# or
node --version
```

### List Locally Installed Node Versions

```bash
nvm ls
```

### List Available Node Versions Remotely

```bash
nvm ls-remote
```

### Install a Specific Version of Node

```bash
nvm install 18.16.1
```

### Set the Default Node Version

```bash
nvm alias default 18.16.1
```

### Switch to a Different Node Version

```bash
nvm use 20.5.1
```

### Install the Latest Long Term Support (LTS) Version of Node

```bash
nvm install --lts
```

### Install the Latest Stable Version of Node

```bash
nvm install stable
```
