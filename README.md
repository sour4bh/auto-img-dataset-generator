auto-img-dataset-generator
===========================

Automatically fetches images from google image search and applies custom defined pre-processes 

### Dependencies:
    selenium    
    requests
    urllib3

Please make sure selenium webdriver is the correct version:
Google Chrome Version -> Selenium Version -> Selenium chrome webdriver driver

install the dependencies by
```
pip install -r requirements.txt
```

### Execute
#### Prepare your image list:
imglist.txt stores the search queries. Multiple search queries can be added on each line.

##### Sample content of imglist.txt
    cat
    dog
    ...

Then execute the downloader by (For windows and Linux)
```
python generator.py --input imglist.txt --output results --size 100 
```

To see all the arguments:
```
python generator.py --help
```

After running, all results will be in 'results' folder, with one folder per query.

### Note:
1. The verison of chrome driver may not fit for chrome version, please check your chrome version and download corresponding driver from [here](https://sites.google.com/a/chromium.org/chromedriver/downloads)
~~2. The number of output images may not be equal to the size option since there could be some invalid url~~
