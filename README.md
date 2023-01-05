# Using Web Scrapping in Google Images


Web Scrapping can be a useful way to obtain raw data if the content needed is scarcy or difficult to get, the way this kind of tools work is by addressing the "visual" data of an URL and getting the information needed, there are many libraries, but the main ones are `BeautifulSoup` that focus in obtaining information by the structure of the webs data with or `Selenium` which is a browser automation library. To get more info, visit this [link](https://medium.com/ymedialabs-innovation/web-scraping-using-beautiful-soup-and-selenium-for-dynamic-page-2f8ad15efe25).

Due to the fact that recently Google Images has changed the way the page refresh and it oblies you to scroll down in order to load more images, I determine that the most suitable library to use would be `Selenium`, imitating the process a user would do to download each image and automize it.

## Way to use it

In order to make it more usable and easy for you, I have made a function with the arguments needed for the proccess. These are:

### Selenium API (`path_api`)

As told, we will lean on a Selenium API of our preferrable Web Browser, so we will have to download it to automate the search, you can find different Selenium drivers [here](https://www.selenium.dev/selenium/docs/api/javascript/index.html). Once we have downloaded the web driver we have to place the path of its location in the `path_api` argument.

### Google searchs (``urls``)

In this argument we will place a list of the different web searchs we will like to download their images. 


### URLs Directories (``directory_names``)

This argument is expected to be another list (with the same length as `urls`) with the names that we want to reffer to the images. These names must be in the same order than the URLs.

### Directory path (``directory_path``)

The location in local where we want to place the different directories created.
