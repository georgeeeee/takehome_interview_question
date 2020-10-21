# takehome_interview_question

This repository includes a `joomla 3.9.22` stable full package and a dump of database tables. This joomla folder is deployed on `WAMPServer 3.2.3` on Windows 10 operation system (the counterpart on MacOS is called `MAMP`) when the website is under development.

## Deployment Steps
1. Install the lastest `WAMPServer`.
2. Put the `Joomla_3.9.22-Stable-Full_Package` folder into `(path_to_wamp64)/www` folder.
3. Left click the `WAMPServer` icon located at the bottom right corner, choose `Your VirtualHost` then click `VirtualHost Management` and fill out the required field to create virtual host.
3. Create a database called 'joomla' in MySQL.
4. Import the `joomla.sql` file into the 'joomla' database.
5. (Optional) Change `configuration.php` by changing the `$user` and `$password` to your MySQL server's username and password.
6. (Optional) Go to System -> System Information -> Directory Permissions to check whether the `Log folder` and the `Temp folder` are writable. If not, then change the `$log_path` and `$tmp_path` parameters to the corresponding ones.

## Joomla Admin Credentials
* username: admin
* password: admin

## Workflow Demo Screenshot
* Welcome Page
![Welcome Page](https://user-images.githubusercontent.com/18320430/96704426-1087f380-1362-11eb-994a-e7b8104065b5.jpg)

* Test Form Page
![Test Form](https://user-images.githubusercontent.com/18320430/96704487-2695b400-1362-11eb-9c6e-f25a8a03ab8c.jpg)

* User Email Notification After Form Submission
![User Notification](https://user-images.githubusercontent.com/18320430/96704551-3a411a80-1362-11eb-9d78-f165f7062352.jpg)

* Administrator Email Notification After Form Submission
![Administrator Notification](https://user-images.githubusercontent.com/18320430/96704565-3f9e6500-1362-11eb-96bc-aa8bcc7348fb.jpg)



##### Reference: [Move a Joomla website to a new server](https://buckleupstudios.com/move-a-joomla-website-to-a-new-server/), [Copying a Joomla website](https://docs.joomla.org/Copying_a_Joomla_website)
