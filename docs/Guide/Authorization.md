---
sidebar_position: 2
---

#### Public Authorization

Most actions can be performed without requiring authentication from a specific user. For example, fetching, or sending a mail does not require a user to log in.

To authenticate requests in this way, pass your application’s access key via the query parameter:

```URL
    https://devmailer.netlify.app/api/sendmail?apikey=YOUR_API_KEY
```

**⚠️Note:**
Keep your API key with you safely, there is no backup in server. If you lost your API key, You have to delete the old accound and create an new account.
