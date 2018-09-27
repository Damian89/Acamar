# Acamar
A Python3 based single-file subdomain enumerator (with barely dependencies; BeautifulSoup is required tho). 

**[1] Another.. Why?**

Because I had some issues with other solutions and always try to expand my own toolset instead of using tools made by other people. You can learn a lot about different things!

**[2] Is it better?**

I doubt, but it enumerates `14 online services` successfully and didn't implement performance-heavy services like *WaybackMachine*, *Archive.is* or *Baidu*. It's neither multi-threaded but finishes every time under a minute. Here is a PRO/CONTRA:

- **Pro:** single-file, Python3 based, low-dependency, no API keys, I will enhance this project ;-)
- **Contra:** single-threaded, probably missing something, no fancy interface stuff, no DNS bruteforce (future release)

**[3] I wanna use it, how?**

```
pip install beautifulsoup4 requests
python3 acamar.py [domain]
```

**[4] Example**

```
python3 acamar.py twitter.com

[..]
service01.dmz1.twitter.com
partnerdata01.dmz1.twitter.com
www01.dmz1.twitter.com
www02.dmz1.twitter.com
spiderduck01.dmz1.twitter.com
spiderduck02.dmz1.twitter.com
spiderduck03.dmz1.twitter.com

[!] Counting 753 unique subdomains
```
The result will be saved in the same directory under a filename called `[domain].txt`
