# takehome_interview_question

This repository includes a `joomla 3.9.22` stable full package and a dump of database tables. This joomla folder is deployed on `WAMPServer 3.2.3` on Windows 10 operation system (the counterpart on MacOS is called `MAMP`) when the website is under development.

## Deployment Steps
1. Install the lastest `WAMPServer`.
2. Put the `Joomla_3.9.22-Stable-Full_Package` folder into `wamp64/www` folder.
3. Create a database called 'joomla' in MySQL.
4. Import the `joomla.sql` file into the 'joomla' database.
5. (Optional) Change `configuration.php` by changing the `$host` parameter to your local host ip address, `$user` and `$password` to your MySQL server's username and password.
6. (Optional) Go to System -> System Information -> Directory Permissions to check whether the `Log folder` and the `Temp folder` are writable. If not, then change the `$log_path` and `$tmp_path` parameters to the corresponding ones.

## Joomla Admin Credentials
* username: admin
* password: admin

##### Reference: [Move a Joomla website to a new server](https://buckleupstudios.com/move-a-joomla-website-to-a-new-server/), [Copying a Joomla website](https://docs.joomla.org/Copying_a_Joomla_website)
