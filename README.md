# Storefront Catalog Service - Postman Collection

### How-to
1. All requests are located in ```queries``` folder. Download ```queries.postman_collection.json```
2. Inside ```environment_variables``` folder there are prod and sandbox environment variables that can be run on the same queries. You can download both files.

3. In Postman application:
    1. from Collections tab, press Import button and select your ```queries.postman_collection.json``` file
    2. from Environments tab, press Import button and select your ```prod.postman_environment.json``` or ```sandbox.postman_environment.json``` file

4. Navigate to Environments tab on the left and click on the available value (sandbox or prod, depending on what you have downloaded on step 2)

5. Complete all the fields with corresponding data from your Magento Instance
    1. ```Magento-Environment-Id``` represents the id of the shop.  </br>
       You can access it from Admin sidebar of your Magento instance by following the path System -> Services -> Commerce Services Connector -> Saas identifier -> Data Space ID
    2. ```Magento-Website-Code``` represents the id of a website from the above shop.</br>
       You can access it from Admin sidebar of your Magento instance by following the path Stores -> Settings -> All Stores
       Default value is set to ```base``` and you can add new websites as needed
    3. ```Magento-Store-View-Code``` represents the locale in which the product is shown.</br>
       You can access it from Admin sidebar of your Magento instance by following the path Stores -> Settings -> All Stores</br>
       Default value is set to English with code ```default``` and you can add other values such as ```french```, ```spanish```, ```yourCustomLocale```
    4. ```Magento-Store-Code``` represents the code of a store from your website</br>
       You can access it from Admin sidebar of your Magento instance by following the path Stores -> Settings -> All Stores
       Default value is set to ```main_website_store```, but you can add more if needed
    5. ```Magento-Customer-Group``` represents a group of customers for which the prices may differ.For example Wholesale customers might have lower prices than Retailer customers</br>
       It can have one of the following values:
        1. "customerGroupCode":"b6589fc6ab0dc82cf12099d1c2d40ab994e8410c","name":"NOT LOGGED IN"
        2. "customerGroupCode":"356a192b7913b04c54574d18c28d46e6395428ab","name":"General"
        3. "customerGroupCode":"da4b9237bacccdf19c0760cab7aec4a8359010b0","name":"Wholesale"
        4. "customerGroupCode":"77de68daecd823babbb58edb1c8e14d7106e83bb","name":"Retailer"

    6. ```x-api-key``` represents the access key provided by Adobe

6. Go to Collections tab and select your query

7. Make sure the Environment is set accordingly (see postman top right corner)
