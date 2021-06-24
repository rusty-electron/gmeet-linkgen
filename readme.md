# gmeet-linkgen

A small python script that uses Google Calendar API to generate Google Meet links.

### How to use:

* install dependencies:

```python
# this installs google client library
pip install --upgrade google-api-python-client google-auth-httplib2 google-auth-oauthlib
```

* enable *Google Calendar API*. Visit [this link](https://developers.google.com/calendar/quickstart/python) and follow the instructions in step 1(on the website) only.

Once you have completed the instructions on the site, download the `credentials.json` file and save it in the same folder as the `linkgen.py` script.

* run the script. On the first run, it will open up a browser window where you need to login/choose a google account through which you shall be joining the meeting. Choose the account and then close the browser window.

*Setup is now complete and you can run the script to get a googlemeet link.*

> After first run, you can delete the `credentials.json` file or save it in a secure location as it is no longer required by the script. The creds are stored by the script in the *token.pickle* file.

### Usage suggestion

I suggest setting up a keybinding to run this script and then use a clipboard manager to pipe the output to your clipboard so that you can directly paste a googlemeet link when needed.

> for xclip users: `python linkgen.py | xclip -selection primary`

### updates
The google api and its related code are modified quite often so it is possible that the script may not work at the time you are reading this. If that is the case then do let me know by creating an issue. I will try to fix it on the upcoming weekend or earlier.
