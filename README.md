# Python : Sending Emails using SMTPLIB
I recently dived into Python 3 as a learning exercise to explore how I could send a batch of emails. In a production setting, there may be more straightforward approaches, but the following worked well for me.

## Installation 
It is built-in module in python. No need of installation.

```python
import smtplib
smtpObj = smtplib.SMTP( [host [, port [, local_hostname]]] )
```

## Contributing
Pull requests are welcome. For major changes, please open and issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
