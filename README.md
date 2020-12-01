# cloudssp

## Searching For Your Site
<p> First U Need to See if you're Target is running cpanel, https://target.com/cpanel
  or use subdomainscanner and see if it has a www.cpanel.target.com if so the target might be vulnerable.</p>

<p> Looks Like the site Does Not Have the Cpanel redirect on the main, lets check the subdomains And looks like we found www.cpanel.target.com, www.webmail.target.com, www.mail.target.com Okay so lets check if they have the service mailman running. www.webmail.target.com/mailman > 404 www.mail.taregt.com/mailman/ > 200 Okay Exploit Time</p>

<img src="https://imgur.com/5OgcSEd.jpg" data-canonical-src="https://imgur.com/5OgcSEd.jpg" style="max-width:50%;">
<img src="https://imgur.com/2sNGZZa.jpg" data-canonical-src="https://imgur.com/2sNGZZa.jpg" style="max-width:50%;">

## Exploiting

```bash
requires > Python3 with requests version 2.19.1.

```

```bash
python3 exploit.py https://target.com/
```
<img src="https://cdn.discordapp.com/attachments/782029993177382942/783058195551748126/Screenshot_20201129-230325_UserLAnd.jpg" data-canonical-src="https://imgur.com/wauxE3l.jpg" style="max-width:50%;">


