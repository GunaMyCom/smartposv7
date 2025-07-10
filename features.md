#  Smartposv7 Features


## Implemented 

* Option for Customer Display
* Support for displaying promotions or advertisements on Second Display.
* Option to add user Access.
* PayIn and PayOut.
* Price Change.
* Hold and Recall the bill.
* Refund.
* Credit Note.
* Foreign currencies exchange option.(Option for including multiple forigen currency prices in the bill).
* Option for Bill Adjustment.(Need's to do based on user access).
* Automatic Cashier Logout.

* Option for discounts.
    * BillWise Discount.
    * Itemwise Discount.
    * Group Discount.
    * SubGroup Discount (Not Implemented).
    * Manual Discount 
* Type of customer Selection options.
    * Delivery.
    * PickUp.
    * Credit Customer.
    * Loyalty Customer.

* Cancel Bill (with reason).
* Void Bill.
* Quick Search Item Screen.

* Local Server Fallback when the main server Down.
* Based on locale need's to print the bill in different languages.

* Daily Stock Checking (Implemented need's to do the downloading part).

# Need's to check 
    * Price Level (Are we need to use price master or item price 1 and 2 and 3 in the item_master table itself).
    * Loyalty.
    * End of day and cash report.


# Integration
* Integration with Call center application


# Pending 
  * Biometric Authentication.
  * Email Notification.


# Confirmation
* Warranty details through Bill printing
* Daily Stock Count (Counter Stock).
* Integration with  Bank card
* Integration with  E commerce
* Integration with Zatca
* Integration with Fiscal printer
* E-Voucher Implementation
* ECR Integration.
* Promotions.


## Tested
 * Customer Display.
 * Second Display.
 * BackGround Video and Photo.
 * Void Bill
 * Cancel Bill.
 * Price Checking.
 * Repeat
 * No-Sale(Cash Drawer Opening).
    Known Issues :
        * When pressing the no sales without the clear option which will try to save the normal bill. 

### Issues 
# Customer Display (Known issues)
    DeadLock happen's.(Unplug and plug) (Unfortuently)

# While scrolling the Lookup bills Need's to fetch use the page count remaining.

# Need's to stable the quick search item lookup screen.

### Today Task
 * Bill Lookup  
    * Hold 
    * Settled Orders
    * History bill's.
* Payout and PayIn bill.
* Price Change
* Enter NFplu Item.
* Entering Quick Search Item (Fplu Item).
* Automatic LogOut.

Implement the feature for email printing 

### Advance Features.
* Refund Items.
* Option for Price Level's.
* Credit Note.
* Printing QR Code within the bill (Need's  to add as the settings).
* Printing Tax Invoice No in the bill print.
* Loyalty Bill.
* Discount Bill.
* Selecting the Order Source and Order Types.


### Need's to do 

* All the price change is associated with the logged in user based on master it will allow or not allow the feature or need to request to high offical to approve.

* As Default Order Type and Bill Type need's to be the IN-STORE.
* Releated to Printer Settings need's to add the below settings


    * Last Eod Date.
        * At the time of eod we need's to note how many items where synced for bill.

    * Last Synced Date. (Downloading from backoffice). (Need's to show how many items where downloaded and for each api call.).

    * Need's to add the validation before saving the bill and printing total item_tot_amt (bill_tran) and Net Amt (bill_header) should be same.  

    * For Validate Access need's to update based on user_access table schema

    * Customer information's need's to show in expandable header.
        * For loyalty customer need to show the loyalty points and amount.