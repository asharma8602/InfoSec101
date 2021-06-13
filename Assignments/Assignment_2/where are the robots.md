# PicoGym Web Exploitation Writeup

Author: [Ashutosh Sharma](https://github.com/asharma8602)

Challenge Page: [where are the robots](https://jupiter.challenges.picoctf.org/problem/60915/)

## Walkthrough

Starting from the inspecting the code of the webpage. First i randomly opened its css file as in one line i saw that some elements were hidden on the page but all that resulted into nothing. Then i saw a commneted line in the html file of the website , which said that google can't see this part of the webpage.Then first thing which clicked my mind was that i googled about this , and found out there are files called robots.txt on webpages , which show that some parts of webpage are restricted to some specified users, then i modified the url of the webpage to `https://jupiter.challenges.picoctf.org/problem/60915/robots.txt` and found out the contents of the robots.txt file which were 
`User-agent: *  Disallow: /8028f.html`.

Still not able to understand those i googled about what the terms mentioned in the robots.txt file meant.Then finally i edited the url properly `https://jupiter.challenges.picoctf.org/problem/60915/8028f.html`

## Flag

`picoCTF{ca1cu1at1ng_Mach1n3s_8028f}`

## Useful resources (if any)


## Suggested modifications [Optional]

What can you do to make this level more difficult. The inherent idea should be similar.
