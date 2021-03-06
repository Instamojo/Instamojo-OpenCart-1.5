# Instamojo Opencart 1.5.X Payment Gateway Plugin

## Download:

Download the zip from [latest release](https://github.com/Instamojo/Instamojo-OpenCart-1.5/releases/latest) section or download it from the [OpenCart Extensions website](http://www.opencart.com/index.php?route=extension/extension/info&extension_id=21984).

## Installation

1. Copy the contents of `upload` directory(the folders inside upload directory in plugin) into your OpenCart installation root directory.
2. Navigate to `Extensions > Payments` from admin panel menu.
3. Look for the Instamojo in Payment List.
4. Click on `[install]` to install it.

## Configuration

1. After installation click on `[edit]` button corresponding to Instamojo module.
2. Fill the following details:

    - **Order Status :** This is the order of the status that you would like to set after a successful payment.

    -  **Checkout Label:** This is the label users will see during checkout, its default value is "Pay using Instamojo". You can change it to something more generic like "Pay using Credit/Debit Card or Online Banking".
      
    -  **Status:** This is the current status of the module. To use Instamojo during checkout make sure to change it to enabled.
     
    - **Client ID** and **Client Secret** - Client Secret And Client ID can be generated on the [Integrations page](https://www.instamojo.com/integrations/). Related support article: [How Do I Get My Client ID And Client Secret?](https://support.instamojo.com/hc/en-us/articles/212214265-How-do-I-get-my-Client-ID-and-Client-Secret-)
    
    - **Test Mode:** If enabled you can use our [Sandbox environment](https://test.instamojo.com) to test payments. Note that in this case you should use `Client Secret` and `Client ID` from the test account not production.

## Migrating from older version

If you were already using older version of our plugin then follow these steps:

1. Uninstall the old Instamojo extension first from `Extensions -> Payments`.
2. Now remove the following files:
   - admin/controller/payment/instamojo.php
   - admin/language/english/payment/instamojo.php
   - admin/view/template/payment/instamojo.tpl
   - catalog/controller/payment/instamojo.php
   - catalog/language/english/payment/instamojo.php
   - catalog/model/payment/instamojo.php
   - catalog/view/theme/default/template/payment/instamojo.tpl

## Support

For any issue send us an email to support@instamojo.com and share the `imojo.log` file. Location of `imojo.log` file is `system/logs/imojo.log`.
