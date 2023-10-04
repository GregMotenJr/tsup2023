## Folders
- `RPi` - Contains scripts that you should run on your always on server. To get the best benefit, consider using a Raspberry Pi or lower power SBC using Linux.
- `SteamDeck` - Contains the installation script for installing the `nfs-utils` package on SteamOS from Arch repos. **Note the version of the `nfs-utils` package before installation. There may be a newer version.**
- `Sunshine` - Contains my `apps.json` file, as well as my `hdr.bat` script. I did not talk about this in my presentation. See https://github.com/LizardByte/Sunshine/issues/848#issuecomment-1416831679 for more details.
- `Tailscale` - Contains my access control policy to ensure only the ports used for remote gaming are allowed on your tailnet.

# Installation Guide

This guide will walk you through installing and setting up Tailscale Up 2023 on your device.

## Step 1: Clone the Repository

First, you need to clone the repository to your local machine. Open your terminal and run the following command:

\`\`\`bash
git clone https://github.com/swthorn/tsup2023.git
\`\`\`

## Step 2: Navigate to the Cloned Directory

Use the `cd` command to navigate to the cloned directory:

\`\`\`bash
cd tsup2023
\`\`\`

## Step 3: RPi Scripts

If you're using a Raspberry Pi or a similar low-power SBC running Linux, you can run the scripts in the `RPi` folder. These scripts should be run on your always-on server. Navigate to the `RPi` directory in the cloned repository:

\`\`\`bash
cd RPi
\`\`\`

There are several scripts in this directory. Each script is designed for a specific purpose. For example, the `install.sh` script installs necessary packages. To run a script, use the following command (replace `<script_name>` with the name of the script):

\`\`\`bash
./<script_name>.sh
\`\`\`

Please note that you might need to give the script execute permissions before you can run it. You can do this using the `chmod` command:

\`\`\`bash
chmod +x <script_name>.sh
\`\`\`

## Step 4: SteamDeck Scripts

Navigate to the `SteamDeck` directory in the cloned repository:

\`\`\`bash
cd ../SteamDeck
\`\`\`

The `install.sh` script in this directory installs the `nfs-utils` package from Arch repos. To run this script, use the following command:

\`\`\`bash
./install.sh
\`\`\`

Please note that you might need to give the script execute permissions before you can run it. You can do this using the `chmod` command:

\`\`\`bash
chmod +x install.sh
\`\`\`

## Step 5: Sunshine Files

Navigate to the `Sunshine` directory in the cloned repository:

\`\`\`bash
cd ../Sunshine
\`\`\`

The `apps.json` file in this directory is used by Sunshine. You can open this file in a text editor to view or modify its contents.

The `hdr.bat` script in this directory is used for handling HDR. To run this script, use the following command:

\`\`\`bash
./hdr.bat
\`\`\`

Please note that you might need to give the script execute permissions before you can run it. You can do this using the `chmod` command:

\`\`\`bash
chmod +x hdr.bat
\`\`\`

## Step 6: Tailscale Files

Navigate to the `Tailscale` directory in the cloned repository:

\`\`\`bash
cd ../Tailscale
\`\`\`

The `access-control-policy.json` file in this directory contains an access control policy to ensure only the ports used for remote gaming are allowed on your tailnet. You can open this file in a text editor to view or modify its contents.


## Pull Requests
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=shields)](http://makeapullrequest.com)
