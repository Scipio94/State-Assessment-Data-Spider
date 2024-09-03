# State Assessment Data Spider

## There are three parts to creating this Spider:

### 1. Importing the proper packagaes:
  - import scrapy
  - from scrapy import Selector
  - import requests as r
  - from scrapy.crawler import CrawlerProcess

### 2. Creating the Spider:
~~~ python
class SpiderClassName(scrapy.Spider):
  name = 'SpiderName'
  def start_requests(self):
    # code here
  def parse(self, response):
    #code here
~~~

### 3. Running Spider
~~~ python
process = CrawlerProcess()  #--> instansiating process
process.crawl(SpiderClassName) #--> telling process which Spider to run
process.start() #--> running spider
~~~
