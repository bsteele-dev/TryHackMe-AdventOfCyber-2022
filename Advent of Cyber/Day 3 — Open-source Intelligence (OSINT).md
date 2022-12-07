## What is OSINT

OSINT is gathering and analysing publicly available data for intelligence purposes.

## OSINT Techniques

### Google Dorks

Google Dorking involves using specialist search terms and operators to find results not usually surfaced with regular search terms.

Some widely used dorks:
- `inurl`: searches for specified text in all indexed URLs
	- `inurl: hacking` to find URLs that contain "hacking"
- `filetype`: search for specific file extensions
	- `filetype:pdf "hacking"`
- `site`: search all indexed URLs for a domain
	- `site:tryhackme.com`
- `cache`: get the latest cached version of site
	- `cache:tryhackme.com`


### WHOIS Lookup

### Robots.txt

The disallow parameter helps bad actors to identify sensitive directories that can be manually accessed and exploited, like the admin panel, logs folder, etc.

### Breached Database Search

Ex [HaveIBeenPwned](https://haveibeenpwned.com/) 

### Searching GitHub Repos

A common flaw by developers is that the privacy of the repository is set as public.



