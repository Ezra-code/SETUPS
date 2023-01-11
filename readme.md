# RVM installtion

sudo apt-get install software-properties-common "Enter"
sudo apt-add-repository -y ppa:rael-gc/rvm "Enter"
sudo apt-get update "Enter"
sudo apt-get install rvm "Enter"
sudo usermod -a -G rvm $USER "Enter"

## RUBY INSTALLATION

rvm pkg install openssl "Enter"
rvm install 2.7.4 --default --with-openssl-dir=$rvm_path/usr "Enter"
rvm list "Enter"

### ruby gems

gem update --system "Enter"
gem install bundler "Enter"
gem install pry  "Enter"
gem list "Enter"


# NVM installation

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash  <Enter>

## Node installation
nvm install --lts



# GIT

sudo add-apt-repository ppa:git-core/ppa "ENTER"
sudo apt update "ENTER"
sudo apt install git  "ENTER"

## CONFIGURE GIT
* Type git config --global color.ui true and press <Enter>
* Type git config --global user.name + <Space> + your name and press <Enter> (Note: this should be your full name, not your GitHub username, in quotes.)
* Type git config --global user.email + <Space> + the email address you used to sign up to GitHub and press <Enter>
* Type git config --global init.defaultBranch main to update the default branch name Links to an external site.to main
* Type ssh-keygen and press <Enter>. For each prompt do not type anything, just continue to press <Enter>. It's particularly important that you do not enter a passphase; you should leave the passphrase empty when prompted. If you enter a passphrase here, you'll have to enter it every time you interact with GitHub (which will happen a lot during the program). You may also run into issues submitting assignments later.
* Type cat ~/.ssh/id_rsa.pub | clip.exe and press <Enter>. This will copy your SSH key to your clipboard
Open the GitHub New SSH key form Links to an external site.(https://github.com/settings/ssh/new Links to an external site.) (Note: you need to be logged in to GitHub to access that link.)