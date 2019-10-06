# LIPD
LinkedIn Profile Downloader

This program downloads a LinkedIn profile and saves it to a folder with the person's name as the file name.
Because LinkedIn saves each profile with the moniker "Profile*", the user is forced to manually rename the file.
*Some files are named "Profile", then "Profile (1)", etc.; others are named "Profile - (insert date/time)"; depends on the user's computer

With this program, the user signs into LinkedIn through a Selenium Chromedriver, which automates the process of manually clicking on the buttons to download a profile.

Python's built in "shutil" and "os" packages allow for the transfer of the newly downloaded profile (with the person's name as the file name) from a previously specified downloads folder to a previously specified destination folder.

For our purposes, we need to extract the person's first and last names, excluding any titles, middle initials, or any other additional text.

Because there are a large number of edge cases for non-standard "first_name last_name" format, the option to manually rename the file is included. The file can be renamed multiple times.
