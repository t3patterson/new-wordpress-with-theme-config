    #New-Proj-Setup

####1 Initiate process in MAMP
Open *MAMP* applicaton and click *Start Web Page* in MAMP application

####2) Create DB for project
In `http://localhost:8888/MAMP/?language=English` 
Go to `Tools >  phpmyadmin` and create db for project 

####3) Download Wordpress Zip File
Download version of wordpress and unzip 

####4) Create Project Directory in LocalHost w/ necessary Wordpress files
In `/Applications/MAMP/htdocs` directory, create a folder with the project name and c+p contents from that are in the `wordpress` folder from the zipfile

####5) Setup Wordpress to `localhost:8888/«project_name»` and configure wp admin/db settings 

####6) Include the theme files
copy `bootstrap_tm` folder and put the folder in `/wp-content/themes/` directory

####7) Import Pages 
download and import the [wp Pages xml file](./bootstrap_pages.wordpress.2015-12-17.xml)