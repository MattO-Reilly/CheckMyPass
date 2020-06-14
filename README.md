# CheckMyPass
Secure Password Checker

CheckMyPass is a secure Password Checker that checks if your password has ever been leaked on the internet. It works by hashing a password (in this case lets say the password is password123) and the connecting with the https://haveibeenpwned.com/Passwords api to see if and how many times your password is found to have been leaked online.
So password123 is hashed to CBFDAC6008F9CAB4083784CBD1874F76618D2A97, It then takes the first 5 letters and requests any hashed password beginning with these 5 letters. 

Hashing a password is irreversible however sending your hashed password out on the internet could pose a security risk because by brute force attempts the password could be found. By sending out the first 5 letters of the hashed password to https://haveibeenpwned.com/Passwords we can keep our password safe and check on our own device. This aninimity is called K-aninimity.

This programme works in the Terminal and is run by entering any number of passwords after checkmypass.py
It will then print out if and how many times your password has been found and whether it recommends that you change your password.

Sample Terminal Command
$python3 checkmypass.py [*args] 
