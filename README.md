# facebook'

a trash facebook osint tool made with the simple code of

import requests
username = (input("State the Username to search: \n"))
print ("=" * 60)
print ("Searching Username: " + username)
print ("=" * 60)

url = 'https://www.facebook.com/' + username
r = requests.get(url)
if r.status_code == 200:
    print ("=" * 60)
    print ("\n")
    print ("Profile found at: " + url)
    print ("\n")
    print ("=" * 60)
if r.status_code == 404:
    print ("Profile not found!")

if r.status_code == 403:
    print ("Server has blocked the connection!")
 
 
 because i know no other code leave comments to help if u want
