# WordPress-vs-Kali
Time spent: **10** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress.

## Report

1. (Required) WordPress 2.5-4.6 - Authenticated Stored Cross-Site Scripting via Image Filename
- [x] Summary: This vulnerability allows remote attackers to create a specially crafted image file name that will inject arbitrary web script.  This abuses the insufficient validation of the file names of uploaded images.
- Vulnerability types: XSS
- Tested in version: 4.2
- Fixed in version: 4.6.1
- [x] GIF Walkthrough:


- [x] Steps to recreate: Create a new media post and upload an image with the following filename format:

```
filename<img src=a onerror=alert(1)>.jpeg
```

2. (Required)WordPress => 4.2 - User Authentication
- [x] Summary:
- [x] Summary: The system was able to find out if any specific username exists or when we login with any username and password as admin
- Vulnerability types: user authentication,
- Tested in version: 4.2
- [x] GIF Walkthrough: 

<img src='https://github.com/snjgrg/WordPress-vs-Kali/blob/master/gif/signin.gif' title='imageGif' alt='imageGif' />


- [x] Steps to recreate:
