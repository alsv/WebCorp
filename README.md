WebCorp
=======

This project aims at providing both tools and infrastructure for user 
tailored corpus analysis projects.

The project combines various web technologies, databases and natural 
language processing tools to provide researchers with the tools to 
create and access specialized corpora. 

# Technologies

* Nginx + fastcgi
* MySQL
* MongoDB
* Python
* Django
* BeautiflSoup
* readability

# Structure
## backend

* data collection
  * rss
  * twitter
  * facebook
  * google plus
  * upload
* data cleaning
  * BeautifulSoup
  * Readability
  * nltk
* data managing
  * monogdb (tagged data)
  * plain text files (raw data)
  * mysql (metadata)
* admin interface 
  * user creation
  * data administration
  * add modules (i.e. taggers)
  * manage database connections
    + mysql (user accounts)
    + mongodb (corpus data, tagged)
    + text files (corpus data, raw)
* data analysis
  * concordancer
  * wordlists
  * sentiment analysis

## fronted

* contributor
  * add data source
  * auto tag data
  * review and edit tagged data
* user
  * concordancer
  * plots
  * basic statistics (nltk)
