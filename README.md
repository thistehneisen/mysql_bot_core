# mysql_bot_core
Base for MySQL bot running on mIRC

MODULES:
- Seen System - http://www.hawkee.com/snippet/8954/
- Stats System - http://www.hawkee.com/snippet/8958/
- Live Status - http://www.hawkee.com/snippet/8962/
- Channel Peak - http://www.hawkee.com/snippet/9025/
- Human Verification - http://www.hawkee.com/snippet/9042/
(search everything, including 3rd party) http://www.hawkee.com/mirc/snippets/search/MySQL+MBC/

DOCUMENTATION:
[] - optional
$m.sqlb() - wraps text into `these`, which is useful in mysql queries
$m.sqle() - escapes string
$m.sqlq() - wraps text into 'quotes', which is useful in mysql queries
$m.dbres(field,database,where,value[,where2,value2]) - returns db result
$m.dbdel(database,where,value) - deletes entry from database
$m.user(field,id/username,value) - returns user information from `users` database
$m.logged(nickname) - returns user id if specified nickname is logged in
- 1.00 STABLE
$m.setting(setting) - returns setting value from `general` database
m.setting setting value - sets setting value in `general` database
$m.encrypt - variable that encrypts sensitive data (must be static, when active users exists)
- 1.12 STABLE
m.modules Module Name|!command|admin(int0/1)

COMMANDS:
!help - no description needed here
!register username password - create an account
!login username password - log in to account
!logout - log out from an account
!profile /nickname/ - profile info about specified nickname or yourself if not specified
!settings password|signature - sets your profile settings
!admin debug|restart|sesdel - administration options (by default level 5+)

* /something/ - optional setting
* Note: you can change command prefix in local $command aliases

REQUIREMENTS:
- http://reko.tiira.net/mmysql/ (mIRC MySQL by Reko Tiira)
- MySQL database with structure that's below.

