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

Note: Also configure the `wp-config` file--**make sure to add debugging**:
```
define('WP_DEBUG', true);
define( 'WP_DEBUG_LOG', true );
define( 'WP_DEBUG_DISPLAY', true );
```


####6) Include the theme files
copy `bootstrap_tm` folder and put the folder in `/wp-content/themes/` directory

####7) Import Pages 
download and import the [wp Pages xml file](./bootstrap_pages.wordpress.2015-12-17.xml)

####8) Importing Custom Post types
1-- Inside **wp_admin panel** , copy and paste the text below into the *Import* dialogue box contained in: `CPT UI  >  Import/Export ` and select 'Import' button

2-- Go to `CPT UI > Add/Edit Post Types` and save the post 

```
{"portfolio":{"name":"portfolio","label":"Portfolio","singular_label":"Portfolio Piece","description":"post type for displaying portfolio items","public":"true","show_ui":"true","has_archive":"false","has_archive_string":"","exclude_from_search":"false","capability_type":"post","hierarchical":"false","rewrite":"true","rewrite_slug":"","rewrite_withfront":"true","query_var":"true","menu_position":"","show_in_menu":"true","show_in_menu_string":"","menu_icon":"","supports":["title","editor","excerpt","trackbacks","custom-fields","revisions","thumbnail"],"taxonomies":[],"labels":{"menu_name":"","all_items":"","add_new":"","add_new_item":"","edit":"","edit_item":"","new_item":"","view":"","view_item":"","search_items":"","not_found":"","not_found_in_trash":"","parent":""},"custom_supports":""}}
```

3-- Configure Custom Field
- **Field Label** : Link
- **Field name**: link
- **Field Type**: text
#WP Configuration Notes -- New projects

####9) Set Front-Page to `Home` and Posts to `Blog` Pages 
in wp-adming panel: *Settings > Reading : 'Front Page Displays'*

####10) Get the boilerplate project plugins
1 - Copy & paste boilerplate wp-plugins to folder .`/wp-content/plugins/`
2 - activate the plugins in wp-admin area


