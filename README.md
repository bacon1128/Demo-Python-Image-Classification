# Turi Create supports：
- macOS 10.12+
- Linux (with glibc 2.12+)
- Windows 10 (via WSL)
# System Requirements：
- Python 2.7, 3.5, or 3.6
- Python 3.7 macOS only
- x86_64 architecture

# How to install Turi Create on Windows 10(via WSL)：
1. Open Powershell as Administrators and run the following command:
```
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```
2. When prompted, restart your computer.
3. Launch the Microsoft Store and search for Linux. Select the Linux distribution of your choice. For this tutorial, we are using the Ubuntu 18.04 LTS distro.
4. Update and upgrade your distros packages. This will take a few minutes.
```
sudo apt update && sudo apt upgrade
```
# Install and setup virtualenv
1. Install dependencies：
```
sudo apt-get install -y libstdc++6 python-setuptools
sudo apt-get install python3-pip 
```
2. Install virtualenv using pip3：
```
sudo pip3 install virtualenv 
```
3. Create a new virtual environment：
```
virtualenv venv
```
4. Activate your virtual environment：
```
source venv/bin/activate
```
# Install Jupyter Notebook & Turi Create in your Vurtualenv
1. Install jupyter notebook in your virtual environment：
```
pip3 install jupyter
```
2. Make sure you are still in your virtual environment (venv). Install turicreate using the following script：
```
pip3 install turicreate
```
