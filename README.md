# Indian Mutual Fund NAV Downloader
Mutual Fund NAV Downloader is a python program that automates process of downloading historic NAVs for previous 5 years of every Indian Mutual Fund through AMFI website.
Dataset of all Indian Mutual Fund NAVs is in this repository as ZIP file along with a script with which to download NAVs in CSV format

## Demo
[Full Demo](https://user-images.githubusercontent.com/11918572/117841130-65597000-b29a-11eb-8289-b41e03f9275c.mp4)

## Why did I create this?
I felt the need of working with some historical NAV data to find any patterns, this was for a big data project

## Instructions
- Install latest Python Programming language
- Change the bdate & edate in the file before running. Please use the same format for the date
- In the git repo folder > Shift + Right Click > Open Cmd/Powershell > python.exe indian-mf-nav-downloader.py

### CSV Dataset download
If you want dataset to be saved only in CSV format then you can use indian-mf-nav-downloader.py script

### CSV & SQL Dataset download
If you want dataset to be saved in CSV & a SQLITE file then use indian-mf-nav-downloader-sql.py script
SQLITE file is like a huge database in a file you can use https://sqlitebrowser.org/ to look into the sqlite file
This is useful because you can also run SQL queries on this database 

## Dataset 
- It's provided in this repository if you want you can download it & use it directly however it's from 01-May-2016 to 30-Apr-2021 
- Ideally try using the growth-direct database which excludes regular schemes
### How to use dataset?
Use bash grep command to search through schemes 
cat all-funds.csv | grep -i Axis | grep -i Large | grep -i Direct
