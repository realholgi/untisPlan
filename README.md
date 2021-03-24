# untisPlan
Scrape the WebUntis API to display a timetable for today and tomorrow

Usage: `node untisPlan.js username password school baseurl`

- school – Name of the school
- username – Your WebUntis username
- password – Your WebUntis password
- baseurl – The WebUntis Host. Example: XXX.webuntis.com

Example: `node untisPlan.js user secret "MGG Karlsruhe" tipo.webuntis.com`

You may want to run this every hour in your crontab and publish the result on your web server.

Example: 
`0 * * * * /home/user/untisPlan.js 8d secret "MGG Karlsruhe" tipo.webuntis.com >  /www/domain.tld/httpdocs/8d.txt`
