# Save Cart And Buy Later

## Overview

Normally, customers access to your store to see your product but they cannot buy it right away for many reasons such as insufficient butget, not enough in stock or out of stock, etc. Next time, when they come back to buy, they have to remember the product name, search and add the quantity they want to buy. Repeating this process creates much inconvenience for customers, consequently can lead to customers abandoning that purchase. 

Mageplaza Save Cart And Buy Later allows customers to save shopping carts/ products they want to buy in the future, thereby saving time and providing a better experience for customers. With this extension, customers can manage and perform some actions at Customer DashBoard such as Save Cart/ Product, Restore, Delete and Share by Link.

## How to download and install

- [Download Mageplaza Save Cart And Buy Later](https://www.mageplaza.com/magento-2-save-cart/)
- [How to Install](https://www.mageplaza.com/install-magento-2-extension/)



## How to Configure

### 1. Configuration

From the Admin Panel, go to `Stores > Configuration > Mageplaza Extensions > Save Cart And Buy Later > General Configuration`

![](https://i.imgur.com/qZT0tRm.png)


- **Enable**: Select **Yes** to turn on the module
- **Button Title**: Set a title for the button which the customer will click to use this feature. Leaving this field blank will receive the default value which is **Save Cart**.
- **Show Button for Guest**: By clicking to this button, Guest customers will be asked to login so that they can save their cart. 
  - Select **Yes** to allow this button to be shown for Guest.
  - Otherwise, select **No**.
- **Show Buy Later Cart Page Link**: Select the position to display the link to **Buy Later Cart**. There are 2 positions that are **Top Link** and **Footer Link**.
- **Allow Sharing**:
  - Select **Yes** to allow customers to copy this link and share **Buy Later Cart** to others. When customer accesses the link shared, Cart/ Product saved at the link will be automatically added to the new cart
  - Otherwise, select **No**.
- **Upload Buy Later Product Icon**: This feature allows you to select icon to replace for "Buy Product Later" phrase when your website is at "Responsive" or "Mobile mode"

![](https://i.imgur.com/nmS08VM.png)

### 2. Edit Customer Form

From the Admin Panel, go to `Customers > All Customers > Edit Customers > Buy Later Notes`

![](https://i.imgur.com/gBfiwFH.png)

- Here, Admin will see 2 grids: **Saved Carts** and **Saved Products**
- In **Saved Carts Grid**, Admin can view all Saved Carts basic information such as **Cart ID, Created Date, Cart Name, Item(s), Description, Total Price, Action**.
  - In the **Action** column, admin can delete any Saved Cart.
- In **Saved Products Grid**, customers can capture all basic information about Saved Products such as **Image, Name, SKU, Amount Change, Quantity, Action**.
  - In the **Action** column, admin can delete any Saved Product.
  
![](https://i.imgur.com/sAkOGnF.png)

### 3. REST API

Mageplaza Save Cart And Buy Later supports using REST API to perform requests such as admin can get information of configuration of Save Cart And Buy Later; customers can use requests related to Save Cart and Save Product sections. 

View requests supports by Mageplaza Save Cart And Buy Later [here](https://documenter.getpostman.com/view/10589000/T1DiEfN8?version=latest)

View REST API guidelines of Magento 2 [here.](https://devdocs.magento.com/guides/v2.4/rest/bk-rest.html). View create tokens guidelines [here](https://devdocs.magento.com/guides/v2.4/get-started/authentication/gs-authentication-token.html).

### 4. GraphQL

#### 4. 1 How to install 

Run the following command in Magento 2 root folder:

```
composer require mageplaza/module-save-cart-graphql
php bin/magento setup:upgrade
php bin/magento setup:static-content:deploy
```

Note: Magento 2 Save Cart GraphQL requires installing [Mageplaza Save Cart](https://www.mageplaza.com/magento-2-save-cart/) in your Magento installation. 

#### 4.2. How to use

To perform GraphQL queries in Magento, please do the following requirements:
- Use Magento 2.3.x or higher. Set your site to developer mode
- Set GraphQL endpoint as `http://<magento2-server>/graphql` in url box, click Set endpoint. (e.g. http://dev.site.com/graphql)
- To view the queries that the Mageplaza Save Cart GraphQL extension supports, click [here](https://documenter.getpostman.com/view/10589000/TVsuC7mq)

## Frontend

### 1. Link to Dashboard

To use this feature, you are required to login to the store's Website.

#### 1.1. Top Link

![](https://i.imgur.com/EmiXK2n.png)

#### 1.2. Footer Link

![](https://i.imgur.com/yTHzaZK.png)


### 2. View Cart Page

When customers want to come back next time to buy the product they are choosing, click on **Buy Product Later**, this product will be moved to **Buy Later Notes Tab** at **Customer Dashboard**

![](https://i.imgur.com/Rv7IMWO.png)

To save the cart, click the **Save Cart** button. After clicking, a **Popup** will appear so that you can enter the **Cart Name** and **Description** information for this Cart.

![](https://i.imgur.com/8B6LLwd.png)

When clicking **Save**, you will be redirected to the **Buy Later Notes** page and successfully saved this Cart.

### 3. Buy Later Notes Tab

![](https://i.imgur.com/EVG1MrY.png)

#### 3.1. Saved Carts

- From **Saved Carts** tab, customers can capture all Saved Carts basic information such as **Cart ID, Date, Cart’s Name, Cart Total, Item (s), Description, Action**.
- In the **Action** column, customers can perform actions such as View, Share, Restore, Delete.
  - **Action View**: Customers can view details of **Buy Later Cart**.
  - **Action Copy Link**: Customers can copy the link and share **Buy Later Cart** for another person.
  - **Action Restore**: Customers will transfer all Items in Saved Cart to the current Shopping Cart.
  - **Action Delete**: Customers can delete Cart.


#### 3.2. View Buy Later Carts

![](https://i.imgur.com/s9IHqXP.png)

- From **View Buy Later Cart** Tab, customers can capture all the basic information about existing shopping cart products: **Product Name, SKU, Image, Price, Quantity, Subtotal**.
- In addition, right here, customers can perform 2 Actions, which are:
  - **Back**: Return to the **Buy Later Carts** page originally
  - **Restore**: Transfer all Items in Saved Cart to the current Shopping Cart.

#### 3.3. Saved Products

![](https://i.imgur.com/bm6mceS.png)

- From **Buy Later Products** tab, customers can capture all the basic information of Buy Later Products like: **Product Name, SKU, Image, Price, Quantity, Subtotal, Action**.
- In the Action column, customers can perform Actions: Share, Restore, Delete.
  - **Action Copy Link**: Customers can copy the link and share this Saved Product to another person.
  - **Action Restore**: Customers will transfer Items in the Saved Products to the current Shopping Cart.
  - **Action Delete**: Customers can delete this Saved Product.
  


