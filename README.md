# dos2unix

issue: 
env: bash\r: No such file or directory in mac

solution:
Mac
brew install dos2unix # Installs dos2unix Mac
find . -type f -exec dos2unix {} \; # recursively removes windows related stuff

Linux
sudo apt-get install -y dos2unix # Installs dos2unix Linux
sudo find . -type f -exec dos2unix {} \; # recursively removes windows related stuff
Make sure that you're using on your Windows your git configured with this:

git config --global core.autocrlf input
This will instruct git to always commit text files with Linux line ending (\n).
