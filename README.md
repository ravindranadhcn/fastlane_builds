# fastlane_builds

First, check if Homebrew is already installed.

$ brew
If Homebrew is not installed, you will see:

zsh: command not found: brew

Homebrew provides an installation script you can run with a single command (check that it hasn't changed at the Homebrew site).

$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
The Homebrew installation script will ask you to enter your Mac user password. This is the password you use to sign in to your Mac.

 Homebrew shows instructions at the end of the installation process:

- Add Homebrew to your PATH in ~/.zprofile:
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"

After you've installed Homebrew, check that Homebrew is installed properly.

$ brew doctor

Find the Xcode Command Line Tools folder
Use the xcode-select -p command to reveal the location of the Xcode Command Line Tools folder.

$ xcode-select -p
You should see:

/Library/Developer/CommandLineTools
