
# Scraper Op

A platform developed for Police Department where police can gather data about an individual from different social media sites that is publicly available.

## Demo

[Video Link](https://github.com/rajprem4214/ScrapperOP)


## Platform Glance


|      Register Page       |       Login Page        |
| :---------------------: | :----------------------: |
| <img src="https://user-images.githubusercontent.com/85401522/222960015-352c17ec-497e-404b-9bd4-11f6840aeb73.png" alt="Register" border="0" width=400> | <img src="https://user-images.githubusercontent.com/85401522/222959969-11a27463-71ef-4d63-90ce-24f007aa1e0f.png" alt="login" border="0" width=400> |

|      Home Page       |   Data Fetched   |
| :--------------------: | :---------------------: |
| <img src="https://user-images.githubusercontent.com/85401522/222960072-dd7b5bd4-8648-455d-9914-fe07dd461782.png" alt="Faa" border="0" width=400> | <img src="https://user-images.githubusercontent.com/85401522/222960161-dd17c303-20a4-416e-b857-50244f95c849.png" alt="meet" border="0" width=400> |

## Table of Contents
  
  - [Features](#features)
  - [TechStack](#techstack)
  - [Installation](#installation)
  - [Appendix](#appendix)
  - [APIReference](#apireference)
  - [Documentation](#documentation)
  - [Optimizations](#optimizations)
## Features

- **Phone Number Scraping**
  - Scrape data associated with mobile number in India. 
  - Get details of the sim location with proper address.
  - Receive data in JSON format.
  - Download data in CSV file.
  - Screen Sharing
- **Tweets Toxicity Detection (X-factor / Flagship)**
  - Archive tweets of an individual and give toxicity details about it.
  - Toxicity details are served on 7 different parameters.
  - Uses Tensorflow Model to detect the toxicity category.
  
- **Twitter Scraper**
  - Search Twitter Account Details by providing username.
  - Extract all the tweets of the individual.
  - Receive data in JSON format.
  - Download data in CSV file.
  
- **Linkedin Scraper**
  - **Extract** data from a LinkedIn profile of a user.
  - Receive data in JSON format.
  - Download data in CSV file.
  
- **Instagram Scraper**
  - **Extract** data from a Instagram profile of a user.
  - Obtain profile image, no. of followers & following and much more.
  - Receive data in JSON format.
  - Download data in CSV file.

- **Facebook Scraper**
  - **Extract** data from a Facebook profile of a user.
  - Obtain profile image, no. of followers & following and much more.
  - Receive data in JSON format.
  - Download data in CSV file.




## TechStack

![Key Technologies Used](https://user-images.githubusercontent.com/85401522/170822301-510d4ab1-0081-4f8c-b6ef-f3c8812c8f3b.png)

1. Front End / Client Side
    - ReactJS 
    - Bootstrap - CSS and other components
    

2. BackEnd Server ( Followed 2 backend architecture to distribute load on servers ):
   - Flask Backend
     - Facebook Scraper - Intakes Facebook username or ID username and scrapes data from user profile dismentaling the site.
     - Twitter Scraper - Intakes Twitter username and scrapes data from user profile dismentaling the site.
   
   - MongoDB Backend
      - Phone Number Scraper - Scrapes data associated with a mobile number.
      - Instagram Scraper - Intakes Instagram username and scrapes data from user profile dismentaling the site.
      - LinkedIn Scraper - Intakes LinedkIn username and scrapes data from user profile dismentaling the site.

3. Data Management (Databases): 
    - MongoDB Atlas - Data management and user details
   
## Installation


### Pre-Requisites:
1. Install Git Version Control
[ https://git-scm.com/ ]

2. Install Python Latest Version
[ https://www.python.org/downloads/ ]

3. Install Pip (Package Manager)
[ https://pip.pypa.io/en/stable/installing/ ]

4. Install MongoDB Compass and connect it to localhost **27017** [ Atlas Connection is quite slow and may not work everytime ]
- Uncomment the following code in app.py to change the connection as per requirement.

  <img src="https://user-images.githubusercontent.com/85401522/183743315-a766d3a9-f7ff-4797-a162-68849f134134.png" alt="Faa" border="0" width=400>




### Clone the project:

```bash
  git clone https://github.com/rajprem4214/ScrapperOP.git
```

Go to the project directory

```bash
  cd ScraperOP
```

**Backend Server:**

Go to backend folder

```bash
  cd backend-python
```
#### Create a Virtual Environment and Activate:

Install Virtual Environment

```bash
  pip install virtualenv
```

Create Virtual Environment:


```bash
  virtualenv venv
```

Go to venv folder and Activate virtual enviroment

```bash
  cd venv
```
Run the following command
```bash
  .\Scripts\activate.ps1
```
Go back to backend folder
```bash
  cd ..
```
Install Requirements from 'requirements.txt'
```bash
  pip install -r requirements.txt
```

Start the backend server

```bash
 flask run
```


Start the other backend server

```bash
 cd FinalKSP
```

Navigate to server folder

```bash
 cd Server
```

Run the following command

```bash
 nodemon index.js
```


**Frontend Server:**

Go to frontend folder

```bash
 cd instaSCRAP
```

Install all dependencies

```bash
 npm install
```
Start frontend server

```bash
 npm run start
```

#### Local Url for Server:

- Frontend is running on http://localhost:3000 
- Backend is running on http://127.0.0.1:5000 and  http://127.0.0.1:8000



## Optimizations

- Reduced time in scraping data by distributing server load to 2 servers.
- In toxicity detection, instead of all tweets, some sorted tweets were passed for faster detection.


## Future Aspects

- Increase API rate limits to seamlessly extract data.
- Use cloud services architecture to improve performance of the platform.
## Authors

- [Prem Raj](https://www.github.com/rajprem4214)
- [Saishwar Anand]
- [Utsav Sinha]
