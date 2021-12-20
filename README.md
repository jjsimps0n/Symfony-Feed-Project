# Symfony-Feed-Project


### Built With

* [Symfony 5.4](https://symfony.com)
* [PHP 7.3.31](https://www.php.net)
* [XAMPP 7.3.31](https://www.apachefriends.org/index.html)


### Installation

1. Download rssfeed.zip file 
2. Exctract project to htdocs.
3. Connect project to your MySQL by changing .env file.
    ```
    Specific change this line:
    
    DATABASE_URL="mysql://YOUR_MYSQL_USERNAME:YOUR_MYSQL_PASSWORD@127.0.0.1:3306/feeds"
    ```
4. Create database with command line
    ```
    php bin/console doctrine:database:create 
    ```
5. Import feeds.sql file with command line
    ```
    php bin/console doctrine:database:import feeds.sql
    ```
7. DONE!

## Usage

###### How to get list of feed summaries for the specific category

If you want to get specific category feeds, you need to pass URL parameter.

```
localhost/rssfeed4/public/?category=YOUR_CATEGORY
```
<br>

###### Command line to create new category from XML file with Shell
```
php bin/console app:create-feed <url> <category>
```




