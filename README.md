# Clone the project
gh repo clone CodeSagePath/web-scrapper-python
cd scrapper
pip install -r requirements.txt


# Install virtual environment
pip install virtualenv


# Run the project in virtualenv
Linux/MacOS: source virtualenv/bin/activate
Windows: ./virtualenv/bin/activate


# Install chrome (in virtualenv)
# (For Ubuntu or Ubuntu Based Linux Distributions)
sudo apt update && sudo apt upgrade -y
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo dpkg -i google-chrome-stable_current_amd64.deb
sudo apt --fix-broken install
rm -rf google-chrome-stable_current_amd64.deb


# Run the project
python3 scrapper <URL> 
        (
            with arguments such as: "-d", "--dark-mode" : "scrape pages in dark mode"
                                "-t", "--timeout" : "specify download timeout in seconds"
                                "c", "--disable-caching" : "disable caching of assets"
                                "-h", "--help" : "get help regarding usage"
        )

Example: python3 scrapper --help
