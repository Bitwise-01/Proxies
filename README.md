### A simple proxy scraper

Get ten random proxies 
```python	
from scraper import Scraper    


if __name__ == '__main__':
scraper = Scraper()    
proxies = scraper.scrape(size=10)  

while proxies.qsize:
proxy = proxies.get()
print proxy
```

Get proxies from Japan
```python
from scraper import Scraper


if __name__ == '__main__':
 scraper = Scraper()    
 proxies = scraper.scrape(country='Japan')
    
 while proxies.qsize:
  proxy = proxies.get()
  print proxy
```

Get three proxies from Japan
```python
from scraper import Scraper


if __name__ == '__main__':
 scraper = Scraper()    
 proxies = scraper.scrape(country='Japan', size=3)
    
 while proxies.qsize:
  proxy = proxies.get()
  print proxy
```


Get SSL proxies
```python
from scraper import Scraper


if __name__ == '__main__':
 scraper = Scraper()    
 proxies = scraper.scrape(protocol='SSL')
    
 while proxies.qsize:
  proxy = proxies.get()
  print proxy
```

Get SOCKS5 proxies
```python
from scraper import Scraper


if __name__ == '__main__':
 scraper = Scraper()    
 proxies = scraper.scrape(protocol='SOCKS5')
    
 while proxies.qsize:
  proxy = proxies.get()
  print proxy
```

Get proxies on port 8080
```python
from scraper import Scraper


if __name__ == '__main__':
 scraper = Scraper()    
 proxies = scraper.scrape(port=8080)
    
 while proxies.qsize:
  proxy = proxies.get()
  print proxy
```