# XPath
//                                                              # to select in xpath
h1, div, span, p                                                # get the tag/elementname you want
[@class=""]                                                     # to select the class/id/attribue in the html
//elementName[@attribue='value']
//elementName[predicate]
()[1]                                                           # add around the xpath to selcect which item you want
()[2]                                                              
()[3]                                                              

# Examples/Position
//div[@class='' or @class='']/p/text()
//div[@class=""]/span
//div[@class=""]/h1
(//div[@class=""]/h1)[1]                                        # to select one element
//a/@href
//a[starts-with(@href, 'https')]                                # search for text at the beginning
//a[ends-with(@href, 'fr')]                                     # search for text at the end// *not supported in xpath ver.1.0
//a[contains(@href, 'google')]                                  # search for text in between
//a[contains(@class 'js-search-input')]
//a[contains(text(), 'France')]
//ul[@id='']/li
//ul[@id='']/li[1]                                              # to get the first item
//ul[@id='']/li[1 or 4]
//ul[@id='']/li[position()=1 or position()=4]
//ul[@id='']/li[position()=1 or position()=last()]
//ul[@id='']/li[position()>1]
//table[@class='table table-striped table-bordered table-hover table-condensed table-list']

# Going Up XPath(Axes)
axisName::elementName
//p[@id='unique']/parent::div
//p[@id='unique']/parent::node()                                # will figure out what is the parent element automatically
//p[@id='unique']/ancestor::node()                              # will return the parent of the parent
//p[@id='unique']/ancestor-or-self::node()                      #
//p[@id='unique']/preceding::node()
//p[@id='unique']/preceding::h1
//p[@id='outside']/preceding-sibling::node()                    # will get the brother element

# Going Down XPath(Axes)
//div[@class='intro']/child::p
//div[@class='intro']/child::node()
//div[@class='intro']/following::node()
//div[@class='intro']/following-sibling::node()
//div[@class='intro']/descendant::node()