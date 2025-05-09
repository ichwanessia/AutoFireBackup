# AutoFireBackup
AutoFireBackup.exe is an application designed to automatically back up Firebird databases and send notifications via email. This guide will help users understand how to configure and use the application effectively.

# Installation
System Requirements
-  Windows operating system
-  Firebird (Full Installation)
-  Internet connection for email notifications

# Installation Steps
-  Download and extract the AutoFireBackup.exe file to your desired directory.
-  Ensure that Firebird is installed and accessible from the system.
-  Edit the config.ini configuration file as needed (see the next section).
-  Run AutoFireBackup.exe through Windows Task Scheduler with the Run with highest privileges option.

# Application Configuration
The application uses the config.ini file to store configuration parameters.

# Parameter Descriptions
Firebird Settings
-  gbak_path – Path to the gbak.exe executable used for database backup.
-  database_folder – Directory where the databases are located.
-  backup_folder – Location to store backup files.
-  username and password – Credentials for accessing the database.
-  max_backup_files – Maximum number of backup files to keep before older ones are deleted.
-  database_list – List of databases to be backed up.
Email Settings
-  smtp_server – SMTP server address for sending email.
-  smtp_port – SMTP port used (e.g., 587 for TLS).
-  sender_email – Email address used to send reports.
-  receiver_email – List of recipient email addresses (multiple addresses can be separated by commas).

# Using the Application
Running the Backup
Run AutoFireBackup.exe. The application will automatically back up the databases listed in config.ini.

# Receiving Notifications
Once the backup is complete, the user will receive an email notification.

# Checking the Log
The application generates a detailed log for each backup process. Check the backup.log file for more information.

# Conclusion
This guide is intended to help users understand how AutoFireBackup.exe works and how to optimize the database backup process. Ensure the configuration file is correctly set up so the system runs smoothly.
