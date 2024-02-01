Sure, I can help you improve and enhance these Google dorks. Here's an enhanced version:

### Broad domain search w/ negative search

```plaintext
site:example.com -www -shop -share -ir -mfa -git -svn -cvs -dockerfile -k8s
```

### PHP extension w/ parameters

```plaintext
site:example.com ext:php inurl:? | inurl:php?id= | inurl:php?name=
```

### Disclosed XSS and Open Redirects

```plaintext
site:openbugbounty.org inurl:reports intext:"example.com" (type:xss OR type:open-redirect)
```

### Juicy Extensions

```plaintext
site:"example[.]com" ext:log | ext:txt | ext:conf | ext:cnf | ext:ini | ext:env | ext:sh | ext:bak | ext:backup | ext:swp | ext:old | ext:~ | ext:git | ext:svn | ext:htpasswd | ext:htaccess
```

### XSS prone parameters

```plaintext
inurl:q= | inurl:s= | inurl:search= | inurl:query= | inurl:keyword= | inurl:lang= inurl:& site:example.com (type:xss)
```

### Open Redirect prone parameters

```plaintext
inurl:url= | inurl:return= | inurl:next= | inurl:redirect= | inurl:redir= | inurl:ret= | inurl:r2= | inurl:page= inurl:& inurl:http site:example.com (type:open-redirect)
```

### SQLi Prone Parameters

```plaintext
inurl:id= | inurl:pid= | inurl:category= | inurl:cat= | inurl:action= | inurl:sid= | inurl:dir= inurl:& site:example.com (type:sqli)
```

### SSRF Prone Parameters

```plaintext
inurl:http | inurl:url= | inurl:path= | inurl:dest= | inurl:html= | inurl:data= | inurl:domain=  | inurl:page= inurl:& site:example.com (type:ssrf)
```

### LFI Prone Parameters

```plaintext
inurl:include | inurl:dir | inurl:detail= | inurl:file= | inurl:folder= | inurl:inc= | inurl:locate= | inurl:doc= | inurl:conf= inurl:& site:example.com (type:lfi)
```

### RCE Prone Parameters

```plaintext
inurl:cmd | inurl:exec= | inurl:query= | inurl:code= | inurl:do= | inurl:run= | inurl:read=  | inurl:ping= inurl:& site:example.com (type:rce)
```

### High % inurl keywords

```plaintext
inurl:config | inurl:env | inurl:setting | inurl:backup | inurl:admin | inurl:php site:example[.]com
```

### Sensitive Parameters

```plaintext
inurl:email= | inurl:phone= | inurl:password= | inurl:secret= inurl:& site:example[.]com
```

### API Docs

```plaintext
inurl:apidocs | inurl:api-docs | inurl:swagger | inurl:api-explorer site:"example[.]com"
```

### Code Leaks

```plaintext
site:pastebin.com "example.com" | site:jsfiddle.net "example.com" | site:codebeautify.org "example.com" | site:codepen.io "example.com"
```

### Cloud Storage

```plaintext
site:s3.amazonaws.com "example.com" | site:blob.core.windows.net "example.com" | site:googleapis.com "example.com" | site:drive.google.com "example.com" | site:dev.azure.com "example[.]com" | site:onedrive.live.com "example[.]com" | site:digitaloceanspaces.com "example[.]com" | site:sharepoint.com "example[.]com" | site:s3-external-1.amazonaws.com "example[.]com" | site:s3.dualstack.us-east-1.amazonaws.com "example[.]com" | site:dropbox.com/s "example[.]com" | site:box.com/s "example[.]com" | site:docs.google.com inurl:"/d/" "example[.]com"
```

### JFrog Artifactory

```plaintext
site:jfrog.io "example[.]com"
```

### Firebase

```plaintext
site:firebaseio.com "example[.]com"
```

### File upload endpoints

```plaintext
site:example.com ”choose file” | inurl:upload "example.com" | inurl:fileupload "example.com"
```

## Dorks that work better w/o domain

### Bug Bounty programs and Vulnerability Disclosure Programs

```plaintext
"submit vulnerability report" | "powered by bugcrowd" | "powered by hackerone" | site:*/security.txt "bounty"
```

### Apache Server Status Exposed

```plaintext
site:*/server-status apache
```

### WordPress

```plaintext
inurl:/wp-admin/admin-ajax.php | inurl:/wp-content/uploads "example.com"
```

### Drupal

```plaintext
intext:"Powered by" & intext:Drupal & inurl:user | inurl:"/user/login" "example.com"
```

### Joomla

```plaintext
site:*/joomla/login | inurl:"/administrator" "example.com"
```
