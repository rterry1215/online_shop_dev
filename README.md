
![Your Online Shop](images/logotype.svg "Your Online Shop")

----------------------------------------------------------------------

# Your Online Shop System V 4.0.0

## Live Demo

Video: https://youtu.be/PD_olszbGWA

Shop with sample products -> [Your Online Shop Demo Shop](https://youronlineshop.net/sample/)

Admin -> (usr/password) webadmin/webadmin, productsadmin/productsadmin


## About

This is a dynamic web app (Single Page Application) for e-commerce. It is build in Node.js and it is using Postgresql.

https://youronlineshop.net


## Installation

If you prefer we offer FREE YOUR ONLINE SHOP installation and hosting service: more info by email.

1. Upload the compressed file to your web server.
2. Unpack it to the desired folder.
3. Install postgresql and create a new postgresql database.
4. Edit database settings at: server/nodejs/cfg/dbcfg.js.
5. Open your terminal at main folder and type: npm install and then npm start. Once the server is running then you can open your web browser (port 8000) and continue with the installation process.

## Support

Please write: melchorherrera@gmail.com


## Getting started

Once Your Online Shop is installed you can open your browser at the corresponding url address. Lets log-in with some of the admin users to make changes: user webadmin for web content and productsadmin for catalog content. Other operations can be done by user systemadmin, and to check customer orders log-in with ordersadmin.

Once editing some content press Intro or click outside of the editable area to save changes.

To edit some features from the checkout process you should log in with systemadmin user and make an order as if you were a customer. Once you get to the checkout step you should be able to edit checkout options.

Some other configuration can be done by editing some files at cfg folder.


## Troubleshooting

If the database connection is not working you may need to check settings at server/nodejs/cfg/dbcfg.js. Also you may need to import manually database content from file: server/utils/pgsqldb.sql.

If the products images can not be uploaded you may need to allow write permisions for catalog-images.


## Themes

Y.O.S. system has a themes feature. Tou can find theme files at client/themes folder.


## More

Multi-shop feature is now available. You can host several stores by adding their settings to the configuration files.

The files server/cfg/dbcfg.js and server/cfg/config.js contains the stores configuration. Store folder inside catalog-image one can be replicated for each site. You must also enable multi-shop by stabishing isSiteUnique: false at server/cfg/default.js.

Now you should be able to access each shop by adding the shop name (label at server/cfg/config.js and server/cfg/dbcfg.js) after the host name: localhost:8000/shopname.
