# Activate
> conda activate virtual_workspace

# Install
> conda install -c conda-forge scrapy==1.6 pylint autopep8 -y
> conda install selenium -y
> conda install ipython

scrapy crawl countries -o population_dataset.json
scrapy crawl countries -o population_dataset.csv            # can be used with excel
scrapy crawl countries -o population_dataset.xml            # rarley used unless clinet ask for it


# clear
> cls
> Ctrl + L

# Will create a new folder in current dir
> mkdir foldername

# To change dir
> cd foldername

# To view a list in the current dir
> dir
> dir /b
> dir /D
> dir /OD
> dir /W
> dir /?
> dir /b > filename.txt