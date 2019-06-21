# Web-Crawler

## Instructions to reproduce the result
- ``` git clone https://github.com/nithinsivakumar/Web-Crawler```
-  cd to the directory where crawler.py is located
## Requirements - Python3
  
  - If you use python2, upgrade to python3 or install python3 and 
    execute all the python commands by python3 instead of python.
    
  - I have python3 as a default python interpreter in my system, so I use
    ``` python crawler.py ```
  - Once python3 is installed, you should be using python3/pip3 instead of python/pip when executing commands

## Dependencies

* pip install validator_collection
* pip install bs4 
* pip install lxml

> Note: If you just installed python3 and python2 is your default interpreter, you may have to use 'pip3 install #lib#'               'instead of just 'pip install #lib#'.
## Execution

1. `python crawler.py -h`
   - would print the usage and give you list of options to be specified as an argument
   
   ```
      Nithins-MacBook-Pro:crawl Nithin$ python crawler.py -h
      usage: crawler.py [-h] [-u URL [URL ...]] [-d DEPTH] [-f]

      optional arguments:
      -h, --help             show this help message and exit
      -u URL [URL ...], --url URL [URL ...]
                             specify the url of the website/s to crawl eg:-
                             https://github.com
      -d DEPTH, --depth DEPTH maximum depth to crawl
                        
      -f, --file            Save output to file
      ```

2. Execute below command to crawl 'github.com' and store the crawled results in the file
   
   `$ python crawler.py -u https://github.com -d 30 -f`
    
    - sample run
        ```
        Nithins-MacBook-Pro:crawl Nithin$ python crawler.py -u https://github.com -d 30 -f
        url ['https://github.com'] depth 2 file True
        Crawl done. Look for the output file at  /Users/Nithin/Desktop/crawl/github.txt
        
        ```

### Optional arguments
- `-u`  Can input one or more urls. All the parent domain crawls will be saved in domain specific filename
- `-f`  Can leave this blank and results will be printed to console.
