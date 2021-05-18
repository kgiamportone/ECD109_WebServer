Originally developed by Hayden Roeder in 2019-2020 WCP24 Capstone Project, edited by Kyle Giamportone for 2020-2021 ECD109 Smart Electric Meter project.

Remote Web Server Installation/ Setup:
  Clone/unzip Remote Web Server Folder
  cd into Remote Web Server 
  Delete node_modules folder and package-lock.json file
  Run “npm install” to install project dependencies 
  Run “node index.js” to begin running Web Server backend (“Listening on port 3001” should appear in terminal)
  In a new terminal window, cd to Remote Web Server then cd into testapp folder
  Run npm install to install front-end dependencies
  Run “npm start” to launch front-end interface, should launch in Chrome or other browser
  Check first terminal window for console log statements to verify connection
Additional Setup Procedures:
  Get a API Key from a Google account and make sure Maps is turned on for the API key settings
  In testapp -> src -> components -> GoogleMapContainer.js go to line 117 where /*INSERT ACTUAL API KEY*/ is commented and insert your API key in double quotes to active Google Maps heatmap in interface

Interface Guide:
  To create an account, go to Create Account tab and enter username, password, 0 for consumer, 1 for utility, or 2 for admin (not currently functioning)
  Utility Interface: log in to a utility (level 1) account
  Use information on the right side of the top of the page to operate Google Maps heatmap. Use Start Playback and Stop Playback buttons to control heatmap animation. 
  Below Google Maps heatmap, The four buttons can be used to Add a Simulated Meter, Add a Physical Meter (smart meter is hard coded to be represented by Meter ID 6), Update the Data, or Delete all the meters in the system.
  In the chart below the buttons in (b), clicking the buttons in the Meter ID column change which meter is displayed in the measurement display chart at the very bottom of the Utility Interface. The buttons in the State column change Meter between running and stopped for data collection. 
  Under the “Meter Assignments” title, the left-hand Update Meter Assignment tab allows for assigning a meter to a specific user in the system as well as giving the meter a geographical location for the heatmap. 
