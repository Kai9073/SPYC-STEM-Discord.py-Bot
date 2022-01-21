**INCOMPLETED**

##### Current progress:
- [x] function to retrieve to-do assignments
- [ ] bot command to send the assignment list
- [ ] bot command to get the timetable
- [ ] ...

the `getAssignmentList()` function in bot.py will retrieve all unsubmitted assignments from Google Classroom and saves to l4.json

**It may take around 1 minute to retrieve the list of unsubmitted assignments** (currently trying to reduce the time)

#### Set-up
- requires: Google API OAuth2 Token (stored as `./token.json`)
- discord bot (token stored in `./secrets.json`)

```js
// secrets.json
{"token":"yourTokenHere"}
```

##### To get google api credentials:
Google Cloud Platform
https://console.cloud.google.com/

Credentials > OAuth2.0 Client ID
(**IMPORTANT: Use 18+ Edu Acc / 13+ Pers Acc**)

In API:OAuthConsentScrn > Test User > Add pycXXXXX@school.pyc.edu.hk

Run once, get redirect uri, set redirect uri, use school acc to log in