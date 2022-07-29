# Commands
A list of popular tools and commands.

Update the system:
```


curl -o rpi_imager.deb https://downloads.raspberrypi.org/imager/imager_latest_amd64.deb -o google_chrome.deb https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb -o vs_code.deb -L http://go.microsoft.com/fwlink/?LinkID=760868 -o get_docker.sh -fsSL https://get.docker.com -o etcher.sh https://dl.cloudsmith.io/public/balena/etcher/setup.deb.sh

sh etcher.sh

sudo apt update && sudo apt upgrade -y

sudo apt install -y neovim git make libc6-dev zsh terminator ./google_chrome.deb nextcloud-desktop x11vnc net-tools ./vs_code.deb ./rpi_imager.deb balena-etcher-electron

sh get_docker.sh
sudo usermod -aG docker $USER

rm ./rpi_imager.deb ./google_chrome.deb ./vs_code.deb ./get_docker.sh ./etcher.sh

sudo reboot
```

