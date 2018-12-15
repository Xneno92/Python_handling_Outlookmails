#your python path
import smtplib
import base64
from email.mime.multipart import MIMEMultipart
from email.mime.text import MIMEText
to = 'Receipients'
gmail_user = 'Username'
gmail_pwd = base64.b64decode("base64_encrypted_password")
smtpserver = smtplib.SMTP("Server_name",SMTP_PORTS)
smtpserver.ehlo()
smtpserver.starttls()
smtpserver.ehlo
smtpserver.login(gmail_user, gmail_pwd)

# Create message container - the correct MIME type is multipart/alternative.
msg = MIMEMultipart('alternative')
msg['Subject'] = "Mail_Subject"
msg['From'] = gmail_user
msg['To'] = to

# Create the body of the message (a plain-text and an HTML version).
text = 
html = """\
'Place Your HTML Code Here'
"""

# Record the MIME types of both parts - text/plain and text/html.
part1 = MIMEText(text, 'plain')
part2 = MIMEText(html, 'html')

msg.attach(part1)
msg.attach(part2)
smtpserver.sendmail(gmail_user, to, msg.as_string())
print 'done!'
smtpserver.close()
