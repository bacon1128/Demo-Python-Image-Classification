# Test Data：
<https://www.kaggle.com/datasets/alessiocorrado99/animals10?resource=download>

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

# Setting password：
1. If you don’t already have a Jupyter folder, or if your Jupyter folder doesn’t contain a notebook configuration file, run the following command:
```
jupyter notebook --generate-config
```
2. Enter password：
```
jupyter notebook password
```
3. Login as root：
```
jupyter notebook --allow-root
```
4. Website
```
localhost:8888
```
# Reference：
1. [如何用Python和深度神經網絡識別圖像？](https://onway2017.wordpress.com/2020/07/17/%E5%A6%82%E4%BD%95%E7%94%A8python%E5%92%8C%E6%B7%B1%E5%BA%A6%E7%A5%9E%E7%B6%93%E7%B6%B2%E7%B5%A1%E8%AD%98%E5%88%A5%E5%9C%96%E5%83%8F%EF%BC%9F/)
2. [turicreate 6.4.1](https://pypi.org/project/turicreate/)
3. [How to install Turi Create on Windows 10](https://medium.com/@malondireads/installing-turicreate-on-windows-10-534e147a4792)
4. [Running a notebook server](https://jupyter-notebook.readthedocs.io/en/stable/public_server.html)
