# Power-MVP
A power app to manage your MVP Contributions easily.


Installation steps in this order -
1. First you need access to the MVP API. To get that, follow the instructions here - https://mvp.microsoft.com/en-us/Opportunities/my-opportunities-api-getting-started  
After you have completed the steps there, you should have these three things with you -  
  a. MVP API Key  
  b. Application Id  
  c. Application Secret  
  You will need these in your custom connector.
  
2. Import the MVP.swagger.json as a custom connector in Power Apps. Use the Application Id and Application Secret in the Client Id and Client secret respectively. Test the custom connector by logging into the microsoft account that you use for your MVP account. This will create a connection that you can the use while importing the app. 

3. Import the PowerMVP_20200309132708.zip file in Power Apps using the import package feature.
During the import, for the MVP connector, choose the connection that you created in step 1.

4. After the import is complete, open the app in edit mode and go to the SettingsScreen to enter all your API keys.
- MVP API key is required
- YouTube and Twitter API are optional
- For Wordpress blog, add the RSS feed URL for your blog (Limitation - only pulls recent posts and stats are not pulled).

Please feel free to submit your feedback as an issue here.

Improvements planned -
1. Pacakge the whole thing as a solution with CDS entity to archive all contribution data, thus having the option to update stats for all contributions with a click of a button.
2. Wordpress API connection to get stats.

Update as of 4:36 PM Eastern Time on 3/9/2020
1. Removed Twitter connector as it wasn't required.

Update as of 4:00 PM on 3/11/2020
1. Modified the flow to get video details of a channel's YouTube videos. It was throwing an error if the videoid started with a special character.
1. Added Twitter handle as an input to the flow. It will otherwise pull all my(@that_API_guy) tweets instead of the user's tweets.
