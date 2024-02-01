# Google Dorks for Bug Bounty and Web Application Security

Explore this curated collection of Google Dorks to enhance your Bug Bounty, Web Application Security, and Pentesting efforts.

## [Live Tool](https://egscan.co/)
![Screen Shot](https://github.com/dragonked2/google/assets/66541902/50c83306-1e64-48fe-8ca2-4044daa72743)


[![Follow @3lyy313 on Twitter](https://img.shields.io/twitter/url/https/twitter.com/3lyy313.svg?style=social&label=Follow%20%403lyy313)](https://twitter.com/3lyy313)

---

### Broad Domain Search with Negative Filters

> `site:egscan.co -www -shop -share -ir -mfa`

### PHP Extension with Parameters

> `site:egscan.co ext:php inurl:?`

### Disclosed XSS and Open Redirects

> `site:openbugbounty.org inurl:reports intext:"egscan.co"`

### Juicy Extensions

> `site:"egscan[.]co" ext:log | ext:txt | ext:conf | ext:cnf | ext:ini | ext:env | ext:sh | ext:bak | ext:backup | ext:swp | ext:old | ext:~ | ext:git | ext:svn | ext:htpasswd | ext:htaccess`

### XSS-Prone Parameters

> `inurl:q= | inurl:s= | inurl:search= | inurl:query= | inurl:keyword= | inurl:lang= inurl:& site:egscan.co`

### Open Redirect-Prone Parameters

> `inurl:url= | inurl:return= | inurl:next= | inurl:redirect= | inurl:redir= | inurl:ret= | inurl:r2= | inurl:page= inurl:& inurl:http site:egscan.co`

### SQLi-Prone Parameters

> `inurl:id= | inurl:pid= | inurl:category= | inurl:cat= | inurl:action= | inurl:sid= | inurl:dir= inurl:& site:egscan.co`

### SSRF-Prone Parameters

> `inurl:http | inurl:url= | inurl:path= | inurl:dest= | inurl:html= | inurl:data= | inurl:domain=  | inurl:page= inurl:& site:egscan.co`

### LFI-Prone Parameters

> `inurl:include | inurl:dir | inurl:detail= | inurl:file= | inurl:folder= | inurl:inc= | inurl:locate= | inurl:doc= | inurl:conf= inurl:& site:egscan.co`

### RCE-Prone Parameters

> `inurl:cmd | inurl:exec= | inurl:query= | inurl:code= | inurl:do= | inurl:run= | inurl:read=  | inurl:ping= inurl:& site:egscan.co`

### High Percentage Inurl Keywords

> `inurl:config | inurl:env | inurl:setting | inurl:backup | inurl:admin | inurl:php site:egscan[.]co`

### Sensitive Parameters

> `inurl:email= | inurl:phone= | inurl:password= | inurl:secret= inurl:& site:egscan[.]co`

### API Documentation

> `inurl:apidocs | inurl:api-docs | inurl:swagger | inurl:api-explorer site:"egscan[.]co"`

### Code Leaks

> `site:pastebin.com "egscan.co"`  
> `site:jsfiddle.net "egscan.co"`  
> `site:codebeautify.org "egscan.co"`  
> `site:codepen.io "egscan.co"`

### Cloud Storage

> `site:s3.amazonaws.com "egscan.co"`  
> `site:blob.core.windows.net "egscan.co"`  
> `site:googleapis.com "egscan.co"`  
> `site:drive.google.com "egscan.co"`  
> `site:dev.azure.com "egscan[.]co"`  
> `site:onedrive.live.com "egscan[.]co"`  
> `site:digitaloceanspaces.com "egscan[.]co"`  
> `site:sharepoint.com "egscan[.]co"`  
> `site:s3-external-1.amazonaws.com "egscan[.]co"`  
> `site:s3.dualstack.us-east-1.amazonaws.com "egscan[.]co"`  
> `site:dropbox.com/s "egscan[.]co"`  
> `site:box.com/s "egscan[.]co"`  
> `site:docs.google.com inurl:"/d/" "egscan[.]co"`

### JFrog Artifactory

> `site:jfrog.io "egscan[.]co"`

### Firebase

> `site:firebaseio.com "egscan[.]co"`

### File Upload Endpoints

> `site:egscan.co "choose file"`

## Dorks Without Domain

### Bug Bounty Programs and Vulnerability Disclosure Programs

> `"submit vulnerability report" | "powered by bugcrowd" | "powered by hackerone"`  
> `site:*/security.txt "bounty"`

### Apache Server Status Exposed

> `site:*/server-status apache`

### WordPress

> `inurl:/wp-admin/admin-ajax.php`

### Drupal

> `intext:"Powered by" & intext:Drupal & inurl:user`

### Joomla

> `site:*/joomla/login`

---

**Medium Articles for More Dorks:**
- [5 Google Dorks Every Hacker Needs to Know](https://thegrayarea.tech/5-google-dorks-every-hacker-needs-to-know-fed21022a906)
- [Uncover Hidden Gems in the Cloud with Google Dorks](https://infosecwriteups.com/uncover-hidden-gems-in-the-cloud-with-google-dorks-8621e56a329d)
- [10 Google Dorks for Sensitive Data](https://infosecwriteups.com/10-google-dorks-for-sensitive-data-9454b09edc12)

**Top Parameters:**
- [Top 25 Parameter](https://github.com/lutfumertceylan/top25-parameter)

**Proviesec Dorks:**
- [Proviesec Google Dorks](https://github.com/Proviesec/google-dorks)
