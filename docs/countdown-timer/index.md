# Countdown Timer

## Overview


In order to increase the accessibility of customers and demand for products, Mageplaza developed the Countdown Timer extension. This module allows admin to add countdown timer displayed on the website for new products or promotional products. There are 2 types of countdown timer which are before the promotion sale and while running the promotion sale. In addition, there are 5 countdown timer templates available for admin to easily select and edit in accordance with the website design.

## How to download and install

- Download Mageplaza Countdown Timer
- [How to Install](https://www.mageplaza.com/install-magento-2-extension/)


## How to use

### Display the countdown for the catalog

![](https://i.imgur.com/MahznQF.png)

### Display countdown timer for none product

![](https://i.imgur.com/v4gyjbD.png)

### Support 5 clock types

![](https://i.imgur.com/C7ol2ln.png)

![](https://i.imgur.com/JJK7YXK.png)

![](https://i.imgur.com/lrcqAK5.png)

![](https://i.imgur.com/6ToUTkJ.png)

![](https://i.imgur.com/yHtEtji.png)


## How to Configuration

From the **Admin Panel**, go to `Content > Countdown Timer > Configuration`

![](https://i.imgur.com/aGnjKM3.gif)

### 1. Configuration

From the **Admin Panel**, go to `Content> Countdown Timer> Configuration`, select **General**

![](https://i.imgur.com/vlLfWer.png)

- **Enable**: Select **Yes** to turn on the module 


### 2. Countdown Timer

From the **Admin Panel**, go to `Content> Countdown Timer> Manage Rules`

![](https://i.imgur.com/LvUqfiz.gif)

- This is where the discount list is displayed.
- From Countdown Timer, admin can capture basic information of Countdown Timer such as ID, Name, Status, Customer Groups, Store View, Priority, Action.
- **Action**:
  - **Delete**: Delete the information on the Countdown Timer page.
  - **Change Status**: Change the status of the selected Countdown Timer.
  - **Edit**: Navigate to the previous Countdown Timer Infomation page.
  - In addition, admin can **Filter, Change Store View, Hide / Display Columns**.


### 3. New/Edit Countdown Timer

From the **Admin Panel**, go to `Content> Countdown Timer> Manage Rules> Add new`


#### 3.1. General

From the **Admin Panel**, go to `Content> Countdown Timer> Manage Rules> Add new`, select **General**

![](https://i.imgur.com/6sJyWSx.png)

- **Name**: Enter a name for Countdown Timer, this is a required field
- **Status**: Select **Enable** to display **Countdown Timer** in **Frontend**.
- **Store View(s)**: Select the store in which Countdown Timer is displayed, you can select multiple stores
- **Customer Group(s)**: Select the customer group for which Countdown Timer will be visible, you can select multiple customer groups.
- **Apply for**: Countdown Timer applies to each option:
  - **None Product Base**: not applicable based on product, the position to show clock will depend on where you put widget (instruction in point 4)
    - Displays two more field **Start countdown date** and **End countdown dates**.

  - **All Products with Special Price**: Countdown Timer displayed on all products with special price at Frontend.
  
  ![](https://i.imgur.com/dQqmAno.png)

  - **Specific Products with Special Price**: Choose to apply to each product with special price.
    - Show more item information **Conditions**
    - You can also choose the catalog to apply Countdown Timer
    
    ![](https://i.imgur.com/PN8Xbv6.png)

  - **Inherit condition from Catalog Rules**: inherit conditions from the catalog rule
    - Show additional **Select Catalog Price Rule** field
    
    ![](https://i.imgur.com/LuQsr4j.png)

- **Priority**: default value is 0. Countdown Timer has smaller Priority numbers will be displayed first at Frontend.


#### 3.2. Display

From the **Admin Panel**, go to `Content> Countdown Timer> Manage Rules> Add new`, select **Display**

![](https://i.imgur.com/HTARtzj.png)


- **Display on**:
  - Select **position** to display the Countdown Timer in Frontend.
  - Only show the **Product View** option when **Apply for = Apply for product base**.
- **Snippet Code**: display the code segment.

  - **CMS Page/Static Block**: Copy and paste the code into the page in which you want to display the Countdown Timer
  - **Phtml file file**: Copy and paste the code into the .phtml file in which you want to display Countdown Timer
  - **Layout file**: Copy the code and insert it into Magento's .xml file or other extensions you want to display Countdown Timer.
  

- **Before Starting Countdown**:


  ![](https://i.imgur.com/LDzl7gv.png)

  - **Enable**: Select **Yes** to display Countdown Timer before product promotion start.
  - **Clock Style**: choose 1 of 5 available timer types.
  
  - **Template on Product View**: Insert the variables `{{clock}}, {{save_amount}} & {{save_percent}}`, allow showing countdown timer at Product View before sales with the default template: 
  
  ```
  <div class="mp-countdown-title">This product is discounting {{save_percent}}</div>
                            {{clock}}
                            <div class="mp-countdown-message">Hurry up!</div>
  ```

    - **Template on Category View**: Insert the variables `{{clock}}, {{save_amount}} & {{save_percent}}` allow showing countdown timer at **Category View** before sales with the default template:
  ```
  <div class="mp-countdown-title">Discounting {{save_percent}}. Hurry up!</div>
                            {{clock}}
  ```

   - In which: 
     - `{{clock}}`: Show clock
     - `{{save_amount}}`: Show discounted amount
     - `{{save_percent}}`: Show discounted percentage


  - **Title Color**: Choose title color displayed above the clock.
  - **Message Color**: Select the color for the message displayed below the clock.
  - **Clock Background Color**: Select the inside background color of the clock.
  - **Number Color**: Select the number of colors displayed.
  - **Text Color**: Select the color for the text inside the clock 

  ![](https://i.imgur.com/UdlulQb.png)
  
- **Time Remaining Countdown**:

![](https://i.imgur.com/U3y0eA2.png)

  - **Enable**: Select **Yes** to display **Countdown Timer** while product is on discount program
  - **Clock Style**: choose 1 of 5 available clock types.
  - **Template on Product View**: Insert the variables `{{clock}}, {{save_amount}} & {{save_percent}}`, allow showing countdown timer at Product View while running sales with the default template: 
  
  ```
  <div class="mp-countdown-title">This product is discounting {{save_percent}}</div>
                            {{clock}}
                            <div class="mp-countdown-message">Hurry up!</div>
<div class="mp-countdown-title">This product is discounting {{save_amount}}</div>
{{clock}}
<div class="mp-countdown-message">Hurry up!</div> .

  ```

    - **Template on Category View**: Insert the variables `{{clock}}, {{save_amount}} & {{save_percent}}` allow showing countdown timer at **Category View** while running sales with the default template:
  ```
 <div class="mp-countdown-title">Discounting {{save_percent}}. Hurry up!</div>
                            {{clock}}
  ```

  - In which: 
    - `{{clock}}`: Show clock
    - `{{save_amount}}`: Show discounted amount
    - `{{save_percent}}`: Show discounted percentage
    
- **Title Color**: Choose title color displayed above the clock.
- **Message Color**: Select the color for the message displayed below the clock.
- **Clock Background Color**: Select the inside background color of the clock.
- **Number Color**: Select the number of colors displayed.
- **Text Color**: Select the color for the text inside the clock 
  
  
### 4. Widget

You can put Countdown Timer anywhere by creating a widget. To generate widget, please do the following steps:

#### Step 1: 
From the **Admin Panel**, go to `Content > Elements > Widget`, select **Add new Widget**

#### Step 2: Select **Type = Mageplaza Countdown Timer**, choose the current theme at **Design Theme**, then click to **Continue**

![](https://i.imgur.com/dViylrH.png)

#### Step 3: Fill in the required information

![](https://i.imgur.com/GR0wGV1.png)

#### Step 4: Select the position to display widget

![](https://i.imgur.com/psMzBmE.png)

#### Step 5: Select rule applying to widget

![](https://i.imgur.com/zQlFV5j.png)

#### Step 6: Save widget and check the store frontend

### 5. Rest API 

Mageplaza Coutdown Timer extension supports Rest API to add data to Countdown Timer. This enables store owers to create, edit, view, delete, manage information of the extension. 
Chi tiết có thể xem tại đây.

View guildlines to create tokens [here.](https://devdocs.magento.com/guides/v2.3/get-started/authentication/gs-authentication-token.html) 

Note: Get Products Guest vs Get Products Mine 
- The field Date will be plused 1 day in comparison with the date in admin setting
For example: **To date** in admin is 2020/09/30 23:59:59; API is 00:00:00. So this equals that the due date is 01/10/2020 

- There are 2 keys: type và id, in which, type has value = 0 and 1. This means Display On = Category and Product Page. 

For example:  type= 1, id= 14 (product id). Countdown Timer of that product is displayed. 

