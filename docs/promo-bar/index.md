# Magento 2 Promo Bar

## Promo Bar Overview

Suppose that you have special promotions or big events coming up, how can you notify your customers about those programs or events? With Mageplaza Promo Bar extension, you can do it with ease. Promo Bar allows you to display one or more advertising bars at different locations and on multiple pages. By that, you can also set the display time for the promo bar. In addition, we also support Promo Bar compatible with our One Step Checkout, Free Shipping Bar. 

## How to download and install Promo Bar

- Download Mageplaza Promo Bar
- [How to Install](https://www.mageplaza.com/install-magento-2-extension/)


## How to Configuration Promo Bar

### I. Configuration

Login to the Magento Admin, go to `Marketing > Promo Bars > Configuration`.

![](https://i.imgur.com/dadTfbp.png)

Admin can also go to `Stores > Configuration > Mageplaza > Promo Bars` to set module configuration.

![](https://i.imgur.com/dI4IcBi.png)

#### 1.1. General

![](https://i.imgur.com/tmYtxUG.png)

- Select **Enable = Yes** to enable the module.
- **Promotion Category**:
  - **Category Name**: Admin enters a name for the promotion. The system will display an error message if left blank.
  - **Action**: Click on the trash icon if you want to delete promotion category.
  - **Add**: Click Add button if you want to create a promotion category.
- **Allow Customer to Close Promo Bar**: Select **No** not to allow customers to close the promo bar.
- **Auto Close Promo Bar After**: Admin set the time period for automatically closing the promo bar
- **Auto-reopen schedule**: admin select the schedule to re-open the promo bar after being closed. 
  - Note: Auto-reopen is activated when customers click **close** button. 

#### 1.2. Display Setting

![](https://i.imgur.com/EmqY7lP.png)

- Select **Enable Multiple Promo Bars = Yes** to allow multiple promo bars to be displayed.
- If you choose **No**, it will hide Number of Promo Bar field.
- **Number of Promo Bar**: Select the display type for promo bar
  - **Separate**: The promo bars are shown separately.
  - **Slider**: The promo bars are shown in the slider.
  
![](https://i.imgur.com/tLooBeM.png)

- **Change Bar Time**: Enter the display time for each promo bar and it is displayed only when **Number of Promo Bar = Slider** is selected above.

### II. Manage Promo Bars

![](https://i.imgur.com/FfxeaeJ.png)

- Here saved all the created Promo Bars.
- At the grid, Admin can view all the basic information of Promo Bar such as **ID, Content, Name, Status, Promotion Category, Position, Start Time, End Time, Priority, Action**.
- Admin can do some of the following actions:
  - **Edit**: Select **Edit** in the **Action** column to edit the information on the edit Promo Bar page.
  - **Delete**: Select promo bar to delete, `Action > Delete`.
  - **Change Status**: Change the promo bar status.
- **Add New Promo Bar**: Create new Promo Bar.

#### 2.1. Create New/ Edit Promo Bar
##### 2.1.1 General

![](https://i.imgur.com/66UDUPY.png)

- **Name**: Set the title for promo bar.
- Select **Status = Enable** to allow promo bar to be applied.
- **Store Views**: Admin selects a store to display promo bar .
- **Customer Groups**: Select groups of customers who can view promo bar.
- **Promotion Category**: Select the promo category to be applied on promo bar.
- **Start Date**: Select the start date of promo bar display.
- **End Date**: Select the end date of the promo bar display.
- **Priority**: Enter the priority for the promo bar. The lower the value is, the higher the priority.

##### 2.1.2. Conditions

Admin chooses the conditions to show promo bar at Checkout Page.

![](https://i.imgur.com/HGRIeBj.png)

##### 2.1.3. Design

![](https://i.imgur.com/NhWe0lp.png)

- **Load Template**: Choose Promo Bar template. The system will show the Preview Promo Bar when admin choose a specific template. 
- **Text Content**: Admin enters content for promo bar.
- **URL Text**: Enter the content displayed for the value `{{url_text}}`.
- **URL**: Assign the link to the URL Text. When customer clicks on the text url will automatically open a new tab with the assigned link.
- **Load Template**: Admin selects the template for the promo bar.
- **Text Content Color**: Select the font color for the content section.
- **Background Color**: Select the background color for the promo bar.
- **URL Text Color**: Select the font color for url text.
- **URL Text Background Color**: Select the background color for the text url.
- **Preview Template**: Click here admin can preview the promo bar template.

##### 2.1.4. Display

![](https://i.imgur.com/2OLoDEA.png)

- **Display Position**: Select the display position of the promo bar.

  ![](https://i.imgur.com/qVjvA44.png)
  - **Top of the page**: promo bar displayed at the top of the page.
  - **Top of the content**: promo bar displayed on the content section.
  - **Fixed bar at the top of the page**: promo bar displayed fixed at the top of the page.
  - **Fixed bar at the bottom of the page**: promo bar displayed fixed at the bottom of the page
- **Custom**: Admin can choose any location in the store to display the Promo Bar by copying and pasting commands into the **CMS page/ Static Block**, **template.phtml file** and store **Layout file**.

![](https://i.imgur.com/8UH2vsS.png)

- **Select Page**: Select the location for displaying the promo bar at the pages.
  - **All Pages**: Promo Bar displayed on all pages.
  - **Specific Page**:
  ![](https://i.imgur.com/sVMMuz5.png)
    - **Display On Page(s)**: Select the page that allows you to display promo bar on. The **One Step Checkout Page** will be displayed here when the admin configure the One Step Checkout extension
    - **Display On Category Page**: Select the category page to display the promo bar on.
    - **Display On Product Page**: Select **Yes** to allow promo bar to display in the product page.


##### 2.1.5. Trigger Setting

![](https://i.imgur.com/7p90Owq.png)

- **Auto-close after**: Admin selects the time to automatically turn off Promo Bar. If you select **Use Config**, the promo bar will apply the time set in the **Configuration** section.

![Imgur](https://i.imgur.com/zFncqk8.png)

- **Auto-reopen schedule**: Admin choose the time to re-display Promo Bar. If you select **Use Config**, the promo bar will apply the time set in the **Configuration** section.

![](https://i.imgur.com/bKgxpyX.png)

### III. Frontend

#### 1. Home page

![](https://i.imgur.com/wu31sss.png)

#### 2. Category Product

![](https://i.imgur.com/Y7D3zvU.png)

#### 3. Product Detail Page

![](https://i.imgur.com/zk7BXOk.png)

#### 4. Check Out Page

![](https://i.imgur.com/dNqNIfp.png)

#### 5. One Step Checkout Page

Promo Bar is fully compatible with One Step Checkout

![](https://i.imgur.com/qXWVGlB.png)

#### 6. Shopping Cart Page

![](https://i.imgur.com/QDc2K6n.png)

#### 7. Compatible with Free Shipping Bar

![](https://i.imgur.com/LIcLRzL.png)

#### 8. Custom

##### 8.1. CMS Page/ Static Block

For example: Admin wants to display Promo Bar on the **About us** page, follow these steps:

- **Step 1**: Go to the backend, click `Content > Pages` and select **Edit** at **About us**.

![](https://i.imgur.com/v2XAY69.png)

- **Step 2**: Insert the code into the page content **About us**.

![](https://i.imgur.com/gXzPgSy.png)

- **Step 3**: Save and check on the frontend

![](https://i.imgur.com/KXkRlPZ.png)

##### 8.2. Template .phtml file

If admin wants to insert a promo bar into a certain location in the **.phtml Template file**, follow these steps:

- **Step 1**: Go to the server and find the directory with the path `vendor/magento/module-catalog/view/frontend/templates`

Below are the folders in the templates file.

![](https://i.imgur.com/BwDF7Sw.png)

- **Step 2**: Select the folder then select the file with the format of **.phtml**

For example: I select the product folder, continue to select `listing.phtml file` to conduct the action

![](https://i.imgur.com/JfauIXT.png)

- **Step 3**: Open the selected `.phtml file` and insert the code

![](https://i.imgur.com/7p2Zs2l.png)

Save and check at the frontend

![](https://i.imgur.com/XB6R6ay.png)

##### 8.3. Layout file

If admin wants to insert a promo bar into a certain location at the **Layout file**, follow these steps:

- **Step 1**: Go to the server and find the directory with the path `vendor/magento/module-catalog/view/frontend/layout`

![](https://i.imgur.com/aqAofPm.png)

- **Step 2**: Select any file and insert the code into the file

For example: I selected the file `catalog_category_view.xml`

![](https://i.imgur.com/rktadWW.png)

Save and check at the frontend.

![](https://i.imgur.com/WZvPNPL.png)

## IV. REST API

Mageplaza Promo Bar supports users in using REST API to add data to Free Shipping Bar. You can add/edit/view/delete the information of the extension. 

View more details [here](https://documenter.getpostman.com/view/10589000/TVKEXxWj).

View guidelines to create Integration Tokens [here](https://devdocs.magento.com/guides/v2.3/get-started/authentication/gs-authentication-token.html)

## V. GraphQL

Run the following command in Magento 2 root folder:

```
composer require mageplaza/module-promo-bar-graphql

php bin/magento setup:upgrade

php bin/magento setup:static-content:deploy
```


To start working with Promo Bar GraphQL in Magento, you need to:

- Use Magento 2.3.x or higher. Set your site to developer mode.
- Set GraphQL endpoint as http://<magento2-server>/graphql in url box, click Set endpoint. (e.g. http://dev.site.com/graphql)
- The queries and mutations that Mageplaza support can be used to view the details [here.](https://documenter.getpostman.com/view/10589000/TVepA8tv)
