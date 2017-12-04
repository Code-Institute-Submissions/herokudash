# Teachta Dála
**Interactive Data visualisation Web Application**

This Web APP is a Code Institute stream 2 projet using Data Visulation to show the Gender, Constituency, Ethnicity, Party and Age of Irish Politicans in the the House Of Representives (Teachta Dála). This project has many uses for visual and interactive journalism. I built this project to show how representitive is the Irish Government for a ever diverse Irish Socitey.

## Live Demo

**Follow this link to view deployed version of the web app https://com-peterkosinski-tddashboard.herokuapp.com/#**

## Built with 
1. Flask 
2. Python
2. HTML
3. CSS
4. Bootstrap
5. MongoDB database
6. JavaScript Libraries:
    * d3.js
    * dc.js
    * crossfilter.js
    * queue.js
7. A dataset obtained [here](https://stats.oecd.org/Index.aspx?DataSetCode=WILD_LIFE#)

## Components



#### Flask
A Python micro-framework that was used to serve the data and render the HTML pages for this Application

#### Python
A Python file name threatened_species.py renders a graphs.html template and builds a web server using pymongo to interact with MongoDB

#### MongoDB database
NoSQL database that converts and presents data in JSON format. The dataset resource was downloaded as a csv file from [here](https://stats.oecd.org/Index.aspx?DataSetCode=WILD_LIFE#) - it had many rows of aggregate data i.e. one row that was the product of three other rows, so it was cleaned and sorted in RoboMongo before being used.

#### Queue.js
An asynchronour helper library for JavaScript

#### Crossfilter.js
A Javascript based data manipulation library that enables two way data binding - you will see this in action when a section of a graph is clicked, all the other graphs filter

#### D3.js
A JavaScript based visualisation engine that renders interactive charts and graphs in svg format when given data, which are then passed in to divs in graphs.html

#### Dc.js
A Javascript based wrapper library for d3.js - this made plotting the charts easier


## Deployment / Hosting

This Application was deployed and is hosted on Heroku - gunicorn Python package runs the http server for the app, the Procfile gives Heroku the information to run the app and requirements.txt is a file that conains all the Python packages (pip installs) required to run the app. mLab MongoDB was chosen to host the dataset on the server.


## Installation

Follow the below instructions to get this project up & running on Mac (commands will be slightly different for Windows)

1. Download MongoDB & Robomongo
2. Go to folder you want to put the cloned project in your terminal & type:
    'https://github.com/PeterKosinski/herokudash.git'
3. Create & Activate a new Virtual Environment in terminal:
    Create: `$ python3 -m venv ~/virtualenvs/name_of_environment`
    Activate: `$ source ~/virtualenvs/name_of_environment/bin/activate`
4. Install the project dependancies:
    `$ pip install -r requirements.txt`
5. Get Mongod running
    `$ mongod --config config/mongoConfig.conf`
6. Open the folder in vscode and use the internal Terminal 
7. Navigate to the 'threatened_species.py', right click and select 'Run python file in terminal'
8. You should see it running below - go to your browser and type '127.0.0.1:5000' into the address bar and the application should appear


## Testing
This Application was tested across a range of browsers
