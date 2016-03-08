**This library allows you to quickly and easily use the SendGrid Web API via Python.**

This library uses the [Sendgrid v2 Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html).

# Installation
Download and extract to your project folder.

# Quick Start

## Setup your credentials

Set your API KEY and Sender Details (If sender is constant) in credentials.py file inside the sendgrid folder.

```python
SENDGRID_API_KEY = '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'
# This is will appear to originate from for your recipient
FROM_NAME = 'Sender'
FROM_EMAIL = 'sender@mail.com'

```

## v2 Mail Send endpoint (Send an Email)

```python
from sendgrid import *

send_via_sendgrid(
    receiver=[{'email': 'john@mail.com', 'name': 'John Doe'}], 
    subject='This is a Subject', 
    html='Html Body',
    plain_text='Text Body', 
    from_name='Dave Doe',
    sender_email='dave@mail.com',
    reply_to='reply_to_email@mail.com'):
```




