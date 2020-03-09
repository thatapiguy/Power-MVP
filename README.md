# Power-MVP
A power app to manage your MVP Contributions easily.


Installation steps in this order -
1. Import the MVP.swagger.json as a custom connector in Power Apps. Test the custom connector by logging into the microsoft account that you use for your MVP account. This will also create a connection that you can the use while importing the app.

2. Import the PowerMVP_20200309132708.zip file in Power Apps using the import package feature.
During the import, for the MVP connector, choose the connection that you created in step 1.

3. After the import is complete, open the app in edit mode and go to the SettingsScreen to enter all your API keys.
- MVP API key is required
- YouTube and Twitter API are optional
- For Wordpress blog, add the RSS feed URL for your blog (Limitation - only pulls recent posts and stats are not pulled).

Please feel free to submit your feedback as an issue here.

Improvements planned -
1. Pacakge the whole thing as a solution with CDS entity to archive all contribution data, thus having the option to update stats for all contributions with a click of a button.
2. Wordpress API connection to get stats.

Update as of 4:36 Pm Eastern Time on 3/9/2020
1. Added twitter handle as an input to the flow. It will otherwise pull all my tweets instead of the user's tweets.
2. removed Twitter connector as it wasn't required.
