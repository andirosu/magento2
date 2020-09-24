<div align="center"><a href="https://netopia-payments.com/"><img alt="Parsedown" src="https://suport.mobilpay.ro/np-logo-blue.svg" width="240" /></a></div>

# NETOPIA Payments module for Magento 2.4
## Options
* Card payment
* mobilPay WALLET

## Installation
The Module placed in folder "Netopia"
1. put **Netopia** folder inside of <your_magento_root>/app/code/
2. SSH to your Magento server and run the following commands
    * <code>php bin/magento setup:upgrade</code>
    * <code>php bin/magento setup:static-content:deploy</code>
    * <code>php bin/magento ca:cl</code>
3.  Complete the **Basic Configuration**   
4. Enable the module from **Advanced configuration**
4. Download your keys from https://admin.mobilpay.ro/ for Live mode and https://sandbox.mobilpay.ro for Sandbox mode.
   Set your Mode at Mode **Configuration** and  Upload the certificates.
   Note : if you would like to have possibility to work with both mode (**Sandbox and Live**), you will need the keys for each mode.


## Verification
By run the following command you can make sure, if this module is installed successfully on your Magento Proiect
* <code>php bin/magento module:status</code>

## After installation
Recommended to firstly, go to Admin panel & fill the necessary data
<code><your_magento_admin>->Stores->Configuration->Sales->Payment Methods->Netopia Payments</code>

* ####Necessary fileds
    * Basic Configuration
        * Merchant Id / Signature
        * Username
        * Password
    * Advanced configuration 
        * Enabled
    * Mode Configuration
        * Live Mode
        
    Note : Except the **Basic Configuration** which is obligatory 
    the other items, will configure with default value, if you don't set them.
