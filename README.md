# Health Provider Scrape

This web scrape utilizes the BeautifulSoup and Selenium Webdriver libraries to fetch the following data from an Anthem Health Provider directory and load it into a CSV file:
- Name
- Address
- Phone #

This script ONLY works for the **Blue Anthem** website. It will break for any other website. 

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for testing purposes. 

### Prerequisites:
- [Python 3.7.0](https://www.python.org/downloads/windows/) 

  Once Python 3.7 is installed:

  - [Webdriver](http://selenium-python.readthedocs.io/installation.html). Please install the **Chrome** version!
    ###### (Copy the path of the installed webdriver! You will need it in set up!)

  - Selenium: 
  
    `C:\Python37\Scripts\pip install selenium`

  - BeautifulSoup: 
  
    `C:\Python37\Scripts\pip install beautifulsoup4`

### Set Up:
1. In the **DriverPath.txt** file, paste the path of the webdriver you installed above

   Example: `C:/Users/johndoe/Downloads/chromedriver`
   
2. If you installed a driver other than **Chrome**, open **Scrape.py** and do the following:
   
   On line 27, by default there is `driver = webdriver.Chrome(path_to_driver)`
   - For **Firefox**: `driver = webdriver.Firefox(path_to_driver)`
   - For **Safari**:  `driver = webdriver.Safari(path_to_driver)`

### Running: 
1. On the command line, go into the directory of this github repository and run:

   `python3 scrape.py`

2. Wait for the scrape to finish, and then open the **OutputData.csv** file and voila, all the health provider data is loaded!

3. Congratulations!
  
### Authors:
- CHUDDY
