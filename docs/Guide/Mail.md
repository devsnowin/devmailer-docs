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

| param   | Description         | Required |
| ------- | ------------------- | -------- |
| from    | Sender name         | true     |
| to      | Recevier email ID   | true     |
| subject | Subject of the mail | true     |
| message | Body of the mail    | true     |

> The form data must be urlencoded data \*

**Note:** message can be <i><u>html</u></i>
