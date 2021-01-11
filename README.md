# logistic-center

This is my CMS course project created in drupal
To install: 
1. clone the repository
2. navigate to the directory with the terminal
3. type `composer install` to install dependencies
4. copy my db and insert in project
5. update vhost:  C:\xampp\apache\conf\extra\httpd-vhosts.conf
    ```<VirtualHost *:80>
    DocumentRoot "C:/xampp/htdocs/drupal/logistic-center"
    ServerName my-drupal.com
    <Directory "C:/xampp/htdocs/drupal/logistic-center">
    Options Indexes FollowSymLinks MultiViews
    AllowOverride all
    Order Deny,Allow
    Allow from all
    Require all granted
    </Directory>
    </VirtualHost>```

Системата е сайт за логистичен център през който може да се добавя пратка както и да се показват всички направени такива.
Пратката има полета Заглавие, от, до, цена, килограми, обем, описание(като потребителите могат да качват и описание като .pdf формат), дата на изпращане която по подразбиране е текущата при създаване на пратката, дата на получаване която по подразбиране е 2 дена след датата на изпращане, има възможност за качване на снимка но тя не е задължителна.
Има възможност за търсене по килограми и по задатено населено място. Използвал съм параграф за създаване на офиси в менюто "за нас",
а Webform съм използвал за контактна форма в същата страница. Използвал съм Content type за създаване на модела на пратката и view(/orderlist) в което се показват всички създадени пратки, там и е формата за търсене която съм създал чрез better exposed filters модула.
За тема съм използвал Drupal8 W3CSS Subtheme 8.x-1.17. 
Не регистрираните потребители имат възможност само да виждат създадените пратки но без да създават такива.
Регистираните потребители ще имат и възможността да създават пратки, както имат и възможност да се свържат с miro logistics.
Използвал съм Pathauto за създаване на custom url.
Custom module позволява на администраторите да добавят често задвани въпроси, а в потребителската част да се вижда само текста публикуван от администраторите.  
 
 Факултетен номер: 20072
 Мирослав Иванов 
 Софтуерно инженерство 4ти курс 
