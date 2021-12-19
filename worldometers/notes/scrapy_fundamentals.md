# Terminal
> scrapy
> scrapy startproject projectname
> cd projectname
> scrapy genspider example www.example.com                      # when pasting the url make sure to remove the "/" at the end of url and the "https" in the front of the url
> scrapy crawl genspidername
> scrapy genspider -l                                           # to view other spiders templates

# Terminal Crawl Spider
scrapy genspider -t crawl genspidername url                     # will have the 'crawl spider' template



# Shell
> scrapy shell                                                  # a good way to practice selecting elements
> scrapy shell "https://www.worldometers.info/world-population/population-by-country/"
>>fetch("https://www.worldometers.info/world-population/population-by-country/")
>>r = scrapy.Request(url="https://www.worldometers.info/world-population/population-by-country/")
>>fetch(r)
>>response.body                                                 # will show html markup
>>view(response)                                                # will open website in browser
>>title = response.xpath("//h1")                                # main way to select elements// response.xpath()
>>title
>>title = response.xpath("//h1/text()")
>>title.get()                                                   # to create a string
>>countries = response.xpath("//td/a/text()").getall()          # will get all the 'a' tags in the 'td' tag in a list
>>countries = response.xpath("//td/a")                          # will outbput a list of elements will make it easy to parse/loop through
>>countries

