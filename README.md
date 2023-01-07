# Using Web Scrapping in Google Images


Web Scrapping its a useful way to obtain raw data if the content needed is scarcy or difficult to get, the way these tools work is by addressing the "visual" data of an URL and getting the information needed. There are many libraries, difering in the method they use, whereas some focus in obtaining information by how the data is  structured (`BeautifulSoup`) others may directly automize a web browser (`Selenium`). To get more info, visit this [link](https://medium.com/ymedialabs-innovation/web-scraping-using-beautiful-soup-and-selenium-for-dynamic-page-2f8ad15efe25).

Due to the fact that recently Google Images has changed the way the page refresh and it oblies you to scroll down in order to load more images, I determine that the most suitable library to use would be `Selenium`, imitating the process a user would do to download each image and automize it.

## Way to use it

In order to make it more usable and easy for you, I have made a function with the arguments needed for the proccess, you can also find it [here](Google_Images.ipynb). These are:

### Selenium API (`path_api`)

As told, we will lean on a Selenium API of our preferrable Web Browser, so we will have to download it to automate the search, you can find different Selenium drivers [here](https://www.selenium.dev/selenium/docs/api/javascript/index.html). To make it simple and don't extend the args too much, we will use chromedriver, **Note that if you want to use another driver, _you will need to change the ``wb`` variable_ in the notebook, placing the API extension** . Once we have downloaded the web driver we have to place the path of its location in the `path_api` argument.

### Google searchs (``urls``)

In this argument we will place a list of the different web searchs we will like to download their images, each item must obviously be an string of the url. 


### URLs Directories (``directory_names``)

This argument is expected to be another list with the names that we want for the directories where the images are going to be located (same length as `urls`). These names must be in the same order than the URLs.

### Directory path (``directory_path``)

The local location where we want to place the different directories created.

## Output

The output when completing the arguments are "n" directories with all the relevant images downloaded from the urls selected
