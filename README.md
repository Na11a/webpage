# webpage
TROUBLESHOOTING
	Проблема при реєстрації
________________________________
SMTPAuthenticationError at /accounts/signup/
(535, b'5.7.8 Username and Password not accepted. Learn more at\n5.7.8  https://support.google.com/mail/?p=BadCredentials t13sm2813998lfp.167 - gsmtp')

1 webpage/setting.py 
1.1 EMAIL_USE_TLS = True
    EMAIL_HOST = 'smtp.gmail.com'
    EMAIL_HOST_USER = 'your_email@gmail.com'
    EMAIL_HOST_PASSWORD = 'your_password'
    EMAIL_PORT = 587
2 Go to your Google Account settings, find Security -> Account permissions -> Access for less secure apps, enable this option.
