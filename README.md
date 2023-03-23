# dorks


# CYBER SECURITY — GOOGLE DORKS

# Finding exposed FTP servers
Google can index open FTP servers. Use the following Google Dork to find open FTP servers.

intitle:”index of” inurl:ftp

To make the query more interesting, we can add the “intext” Google Dork, which is used to locate a specific word within the returned pages

# Find email lists
It is relatively easy to find email lists using Google Dorks. In the following example, we are going to find text files that contain email lists.

filetype:txt inurl:”email.txt”

# Live cameras We can use Google to find open cameras that are not access restricted by IP address. The following Google dorks retrieve live cameras web pages.

inurl:”view.shtml” “Network Camera”

# Finding passwords
Finding passwords is the most attractive task for both legitimate and ill-intentioned online searchers. The following Google Dorks retrieve exposed passwords.

site:pastebin.com intext:admin.password (find the text “admin.password” in the Pastebin website; this site is used by hackers to publish sensitive leaked information)’

“admin_password” ext:txt | ext:log | ext:cfg (find the text “admin-password” in exposed files of the following types: TXT, LOG, CFG)

filetype:log intext:password after:2016 intext:@gmail.com | @yahoo.com | @hotmail.com (search for all files of type “log” that contain the word “password” within them, are indexed after 2016, and contain any of the following text in their body: @gmail.com, @yahoo.com, or @hotmail.com)

# OTHER DORKS LIST -github source

site:static.ow.ly/docs/ intext:@gmail.com | Password
filetype:sql intext:wp_users phpmyadmin
intext:”Dumping data for table orders"
“Index of /wp-content/uploads/backupbuddy_backups” zip
Zixmail inurl:/s/login?
inurl:/remote/login/ intext:”please login”|intext:”FortiToken clock drift detected”
inurl:/WebInterface/login.html
inurl:dynamic.php?page=mailbox
inurl:/sap/bc/webdynpro/sap/ | “sap-system-login-oninputprocessing”
intext:”Powered by net2ftp”

