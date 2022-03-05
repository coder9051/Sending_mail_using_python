# My First Project
I recently dived into Python 3 as a learning exercise to explore how I could send a batch of emails. In a production setting, there may be more straightforward approaches, but the following worked well for me.

So, let's say you have a list of contacts with their names and email addresses. And you'd like to send a message to each of those people, with the phrase "Dear [name]" at the head of the message.

You can save the contact information in a file rather than a database for ease of use. You can also save a file with the message template you want to send.

## Basic Steps :
Here are four basic steps for sending emails using Python:

      1. Set up the SMTP server and log into your account.
      2. Create the MIMEMultipart message object and load it with appropriate headers for From, To, and Subject fields.
      3. Add your message body.
      4. Send the message using the SMTP server object.
      
Let me now take you through the entire procedure.

## SMTP
Simple Mail Transfer Protocol (SMTP) is a protocol, which handles sending e-mail and routing e-mail between mail servers.

Python provides smtplib module, which defines an SMTP client session object that can be used to send mail to any Internet machine with an SMTP or ESMTP listener daemon.

Here is a simple syntax to create one SMTP object, which can later be used to send an e-mail −

```python
import smtplib

smtpObj = smtplib.SMTP( [host [, port [, local_hostname]]] )
```
Here is the detail of the parameters −

       1. host − This is the host running your SMTP server. You can specify IP address of the host or a domain name like tutorialspoint.com. This is optional argument.
       2. port − If you are providing host argument, then you need to specify a port, where SMTP server is listening. Usually this port would be 25.
       3. local_hostname − If your SMTP server is running on your local machine, then you can specify just localhost as of this option.

An SMTP object has an instance method called sendmail, which is typically used to do the work of mailing a message. It takes three parameters −

       1. The sender − A string with the address of the sender.
       2. The receivers − A list of strings, one for each recipient.
       3. The message − A message as a string formatted as specified in the various RFCs.
       

