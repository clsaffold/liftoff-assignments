# Project Outline

### Overview
Since 2012 I have worked closely with healthcare organizations to implement high quality lower cost care delivery models that promote both patient and care team satisfaction.
The tools and many of the tactics we use to achieve this aim are nearly universal accepted despite a very limited body of quantitative data to support their efficacy.
This application will bring together widely accepted Advanced Primary Care best practices, core clinical quality measures and standard quality improvement activities to allow organizations to track the correlation between their change initiatives and outcomes achieved.
A standard set of evidence-based comprehensive care aims, driver and tactics with corresponding measures will be developed and incorporated into an existing Measures Database.
Practices will be able to enter their rapid cycle plan-do-study-act (PDSA) project details, tying them with their pre-defined aims and capturing their intended impacts through measures.
Practice quality improvement facilitators (PF) will be able to log their interactions with practices and connect their notes with practice PDSA entries.
Finally, practices or PFs will be able to upload .csv files containing measures to be ingested into the existing  Measures Database to demonstrate the results of practice change initiatives.
No other fully comprehensive and widely available tool exists to support primary care practices in their efforts to demonstrate return on investment and value of work to continually improve care delivery.
This suite of features will advance the ability of primary care to show tremendous reduction of total cost of care along with improved quality when the investment primary care is increased.
(For liftoff I am focused on PDSA Tracker and .csv file import/data ingesting)

### Features
PDSA Tracker (Main Project)
	User Login: User will be able to log-in by creating accounts in the system or through a token passed from healthteamworks.org drupal membership platform using SAML SSO authentication
				Each user will have a profile page and dashboard of their PDSAs
	Create, edit, append and delete PDSA: Users will be able to create,edit, append and delete their PDSA entries when logged in
	Set Privacy of PDSA: Users would be able to keep their PDSAs private, share them with others in their organization/company or make them publicly viewable
	View PDSAs: Users will be able to view their own PDSAs on their dashboard
	Search: Users will be able to search their own PDSAs and any shared with their org/company and all that are public viewable
	Favorite: Users will be able to mark PDSAs they want to follow as a favorite. These will show up on the user dashboard. 
	Analytics: Each PDSA will display the number of users who have marked it as a favorite.
Measures Database (High Priority Next Project)
	User upload: This feature is already present but only stores the file not the data in the file.
	Data import from .csv files: When users import a cvs file the data can be added to the measures database by period, measure numerator and measure denominator
PF Log
	User Login: SSO authentication with our Drupal-based user directory based on email address. Each user will have a profile page and dashboard of their Practices and Log entries
	Create Log: Users will be able to create a log entry when logged in
	Edit Log: Users will be able to edit a Log entry when logged in
	Search: Users will be able to search all PF logs by Aim, driver, tactic, measure, practice and other fields
	Analytics: Need a way to summarize the logs that correspond to organizations that ultimately achieved the aim they were working toward.
Interactive Change Package (Only Database for Purposes of Liftoff)

### Technologies
C#
Razor
MySQL
SQL
ASP.NET Identity
Web APIs
Security Assertion Markup Language (SAML) Single Sign-on (SSO) miniOrange
DevExpress UI

### What I'll Have to Learn
How to set up authentication and authorization in the app for new users and four authorization levels
		https://docs.microsoft.com/en-us/aspnet/core/security/authorization/secure-data?view=aspnetcore-5.0
How to make one drop-down field's options populate based on what was selected in the previous field
Transform data while importing to properly format all entries in all fields (Advanced)
Add data visualization to the PDSA page based on time-limited entries
Enter data using forms in the app that save the information into two separate databases or how to send all data to one database and then share certain 
	data by API to another database 

### Project Tracker
https://trello.com/invite/b/eulg84Wd/1daed32e38735fe81e8521e92c9b9969/cecilia-liftoff-project-board
