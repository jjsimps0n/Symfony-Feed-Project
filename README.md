# Symfony-Feed-Project


### Built With

* [Symfony 5.4](https://symfony.com)
* [PHP 7.3.31](https://www.php.net)
* [XAMPP 7.3.31](https://www.apachefriends.org/index.html)


### Installation

1. Download project .zip folder
2. Exctract project to htdocs.
3. Connect project to your MySQL by changing .env file.
    ```
    Specific change this line:
    
    DATABASE_URL="mysql://YOUR_MYSQL_USERNAME:YOUR_MYSQL_PASSWORD@127.0.0.1:3306/feeds"
    ```
4. Create Database with feeds.sql file code.
5. DONE!

## Usage

###### How to import XML RSS

To import http://www.feedforall.com/sample.xml XML file into database use url

  ```
  localhost/rssfeed4/public/importfeed
  ```
  > You should receive message ``` Successfully imported new feed, with id: {NEW FEED ID} ```

  After that feed will show at ` localhost/rssfeed4/public ` page table.

<br>

###### How to get list of feed summaries for the specific category

If you want to get specific category feeds, you need to pass URL parameter.

```
localhost/rssfeed4/public/?category=YOUR_CATEGORY
```
<br>

###### Command line to create new category with Shell
```
php bin/console app:create-feed <url> <category> <titile>
```




