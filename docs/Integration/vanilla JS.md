---
sdibar_position: 1
---

Integrating Dev Mailer with a simple form in vanilla JS.

## Get all input data from the form

```javascript
const senderName = document.querySelector("#senderName");
const to = document.querySelector("#to");
const subject = document.querySelector("#subject");
const message = document.querySelector("#message");
```

## Create a function that sends an email

```javascript
function sendMail(e) {
  e.preventDefault();

  var urlencoded = new URLSearchParams();
  urlencoded.append("from", senderName.value);
  urlencoded.append("to", to.value);
  urlencoded.append("subject", subject.value);
  urlencoded.append("message", message.value);

  const options = {
    method: "POST",
    body: urlencoded,
  };

  fetch("http://localhost:3001/api/sendmail?apikey=YOUR_API_KEY", options)
    .then((response) => response.text())
    .then((result) => console.log(result))
    .catch((error) => console.log(error));
}
```

## Select the form and add an event listener to it

```javascript
document.querySelector("#myform").addEventListener("submit", sendMail);
```
