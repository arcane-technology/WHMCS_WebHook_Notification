# WHMCS WebHook Notification
Simple WebHook notification module for WHMCS

### Installation
1. Create a webhooks directory in WHMCSINSTALLDIR/modules/notifications/
2. copy all files into new directory
3. In WHMCS, System Settings -> Notifications. Click Configure on the new WebHooks module, then Save Changes
4. Create a notification rule and choose Webhook in the notification settings
5. Enter the URL for the endpoint you wish to be notified

### Notes
Due to limitations in the WHMCS notification system, data available to send is very limited. As such, details such as ID's, client data, order data etc, is not sent. Only a notification that an event has occured. The receiving system could parse this notification to extract information and then subsequently make an API call back to WHMCS to get more details.

