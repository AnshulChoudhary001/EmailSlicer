Email Slicer with Python
To create an email slicer with Python, our task is to write a program that can retrieve the username and the domain name of the email. For example, look at the image below which shows the domain and username of “support@thecleverprogrammer.com”:

email slicer with Python
So we need to divide the email into two strings using ‘@’ as the separator. Let’s see how to separate the email and domain name with Python:




email = input("Enter Your Email: ").strip()
username = email[:email.index("@")]
domain_name = email[email.index("@")+1:]
format_ = (f"Your user name is '{username}' and your domain is '{domain_name}'")
print(format_)
