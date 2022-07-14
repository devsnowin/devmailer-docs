---
sidebar_position: 4
---

Send mail by providing the required parameters.

## End point

```
https://devmailer.netlify.app/
```

## Send mail

Send a mail

```Request
GET /api/sendmail
```

#### Parameters

| param   | Description         |
| ------- | ------------------- |
| from    | Sender name         |
| to      | Recevier email ID   |
| subject | Subject of the mail |
| message | Body of the mail    |

**Note:** message can be <i><u>html</u></i>
