# Perform Nmap Scan and Export to XML

Perform Nmap Scan and Export to XML:

sudo nmap -oX myscan.xml [target]

Replace [target] with the IP address or hostname of your scan target.

# nmap-converter
Python script for converting nmap reports into XLS
# Requirements
```bash 
sudo pip install python-libnmap
sudo pip install XlsxWriter
```
or 
```bash 
sudo pip install -r requirements.txt
```
# Usage
```bash
usage: nmap-converter.py [-h] [-o XLS] XML [XML ...]

positional arguments:
  XML                   path to nmap xml report

optional arguments:
  -h, --help            show this help message and exit
  -o XLS, --output XLS  path to xlsx output
```

# Example Script Calls

python nmap-converter.py -o myreport.xlsx myscan.xml

python nmap-converter.py -o mycombinedreport.xlsx scan1.xml scan2.xml scan3.xml
