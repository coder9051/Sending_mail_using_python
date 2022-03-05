# Python : Sending Emails using SMTPLIB
I recently dived into Python 3 as a learning exercise to explore how I could send a batch of emails. In a production setting, there may be more straightforward approaches, but the following worked well for me.

So, let's say you have a list of contacts with their names and email addresses. And you'd like to send a message to each of those people, with the phrase "Dear [name]" at the head of the message.

You can save the contact information in a file rather than a database for ease of use. You can also save a file with the message template you want to send.

## Installation 
It is built-in module in python. No need of installation.

```python
import smtplib
smtpObj = smtplib.SMTP( [host [, port [, local_hostname]]] )
```

## Contributing
Pull requests are welcome. For major changes, please open and issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
