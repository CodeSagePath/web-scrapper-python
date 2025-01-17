# Web Scrapper Python Project

## Clone the Project
```bash
gh repo clone CodeSagePath/web-scrapper-python
cd scrapper
pip install -r requirements.txt
```

## Install Virtual Environment
```bash
pip install virtualenv
```

## Run the Project in Virtualenv
- **Linux/MacOS:**
  ```bash
  source virtualenv/bin/activate
  ```
- **Windows:**
  ```bash
  ./virtualenv/bin/activate
  ```

## Install Chrome (in Virtualenv)
### For Ubuntu or Ubuntu-Based Linux Distributions
```bash
sudo apt update && sudo apt upgrade -y
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo dpkg -i google-chrome-stable_current_amd64.deb
sudo apt --fix-broken install
rm -rf google-chrome-stable_current_amd64.deb
```

## Run the Project
```bash
python3 scrapper <URL>
```

### Arguments:
- `-d`, `--dark-mode` : Scrape pages in dark mode
- `-t`, `--timeout` : Specify download timeout in seconds
- `-c`, `--disable-caching` : Disable caching of assets
- `-h`, `--help` : Get help regarding usage

### Example:
```bash
python3 scrapper --help
```
