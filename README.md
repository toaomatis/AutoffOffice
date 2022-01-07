# AutoffOffice
Microsoft Power Automate scheduled cloud flow to automatically set Automatic Replies in case of Out of Office.

## Power Automate
### Sign in
Head over to [Microsoft Power Automate](https://powerautomate.microsoft.com/) and click `Sign in` in the top right corner. This will take you to your companies sign in page.

![Power Automate - Sign in](images/pa_sign-in.png)

### Create a new flow
After a successful login, you will be redirected to the Power Automate landing page. At the left hand side of the screen, you will see a menu. Click the `Create` button. 

![Power Automate - Create](images/pa_create.png)

In the `Start from blank` section choose the `Scheduled cloud flow` button.

![Power Automate - Scheduled cloud flow](images/pa_scheduled-cloud-flow.png) 

### Build a scheduled cloud flow
You are confronted with a pop-up to build your scheduled cloud flow:

1. Give your flow a name. I chose `AutoffOffice`.
2. Choose a starting date. The provided default is fine.
3. Set the interval to `1 Hour`. This will run the flow every hour.
4. Finally, press the `Create` button.

![Power Automate - Build a scheduled cloud flow](images/pa_build-a-cloud-flow.png)

## AutoffOffice flow
At last, you can build an configure your AutoffOffice flow.

First we will take a brief look into the steps the flow will take in order to achieve its goal.

1. Initialize and set variables
2. Get events from your Outlook Calendar
3. Check if events apply for Automatic Replies
4. Enable or disable Automatic Replies based on previous checks

