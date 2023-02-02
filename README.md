## USERWERK Shopify popup plugin

### installation process

Plugin works out of the box with Shopify.checkout object. But if you want to use webhooks also, go to partners.shopify.com, then App setup -> Protected customer data access and check for have all necessary permissions to receive and process clients personal data.

Then go to the folder where docker-compose.yml stores and run "docker-compose up", then go inside www/ and run "composer install". After that all dependencies will be created. 
After host your plugin or run ngrok don't forget change URLs.

Then connect with store owner to grant you access for the store. Then chose this store inside plugin Overwiew  page Select sotre btn. Click install and go through installation process.

### plugin admin panel on the store

After installation is complete you will be redirected to admin panel where you can switch on/off popup window on thank-you page or setting up plugins domain address. Note that shopify-token.txt will be also created, this file keeps store data so keep it in .gitignore and don't provide its content to the third party.
```
for "chocoala.staging.userwerk.com/uw.js"  

Domain will be "chocoala"
```
Default value of domain - "chocoala", of popup visibility - true


### References

Plugin is made on the basis of Shopify recommended library https://github.com/Shopify/shopify-api-php.
Read its docs for receiving more information. So in case of need use this documentation or contact http://innowise-group.com
