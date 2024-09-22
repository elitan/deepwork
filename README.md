# Deep Work Mode

A simple bash script to boost productivity by blocking distracting websites, inspired by Cal Newport's concept of "[Deep Work](https://www.amazon.se/Deep-Work-Focused-Success-Distracted/dp/1455586692)".

## Features

- Blocks specified websites to enable focused work sessions
- Easy to activate and deactivate
- Backs up original hosts file for easy restoration

## Installation

Use this one-liner to download, make executable, and install the script:

```bash
curl -sSL https://raw.githubusercontent.com/yourusername/deepwork-mode/main/deepwork.sh | sudo tee /usr/local/bin/deepwork > /dev/null && sudo chmod +x /usr/local/bin/deepwork
```

This command downloads the script, saves it as `deepwork` in `/usr/local/bin/`, and makes it executable.

## Usage

To start DeepWork mode:
```
deepwork
```

To stop DeepWork mode:
```
deepwork stop
```

## Customization

Edit the `WEBSITES` array in the script to customize blocked sites:
```bash
sudo vim /usr/local/bin/deepwork
```

## Note

- Requires sudo privileges to modify the hosts file.
- The installation script uses `sudo`, so you may be prompted for your password.
- Always review scripts before running them with sudo privileges.
