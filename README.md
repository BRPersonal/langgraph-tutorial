# langgraph-tutorial
Code sample from https://realpython.github.io/gh-download/?url=https%3A%2F%2Fgithub.com%2Frealpython%2Fmaterials%2Ftree%2Fmaster%2Fpython-langgraph

Add the following entries in your .env file
OPENAI_API_KEY=your-api-key

changes done by me  
-------------  

Added utils/AppConfig.py 

ran the command 
pip install python-dotenv

manually modified requirements.txt to add this line
python-dotenv==1.0.1

Run the code. This is the starting point
python graph_demo.py

17-Apr-25
---------
Ran these commands
pip install google-api-python-client google-auth-httplib2 google-auth-oauthlib
pip freeze > requirements.txt


Added file google-calendar-agent.py which pulls meetings in my google calendar for this week
You can run the following natural queries
What meetings do I have this week?
What meetings do I have today?

You need to drop the google oauth client credential json file
in the current folder in the name google_calendar_credentials.json

When you run the program for the first time, a browser window
will open where you have to grant permission to google oauth app
that can access your calendar. Once auth flow is suceesful,
token.json file will be created in local folder.
for subsequent api calls token.json will be used and user will 
not be prompted for google account selection

 
