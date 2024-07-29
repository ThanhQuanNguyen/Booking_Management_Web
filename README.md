# Booking_Management_Web

## Prepare
Tools used: Vscode, Python, HTML, SQLite. Make sure you have every tools installed before installing and running FLaskAPI code folder.

## Activate ETL and SQLite Database
1. Use __"pip3 install - r equirement.txt"__ to install all the necessary packages.
2. Type __"flask db_create"__ into the Vscode Terminal to create database. If it somehow does not work, make sure that there is __sqlite__ installed on your local device. Then __"flask db_drop"__ to drop the databse and __"flask db_create"__ again.
3. Type __"python run.py"__ to start the ETL process. Wait until all the successful annoucements exists.
4. Open __sqlite__ . Go "Open database", click on __booking.db__ to check if the data was created successfully.

## Activate flask API
5. After having database, type on the Vscode Termninal the command __"flask db_seed"__ to seed all the user accounts.
6. Type __"python app.py"__ to activate the flask API.
7. There will be a link existed on the Terminal, __Ctrl+click__ on the link. The Browser will be openned.
8. On the browser, there is a text line "Welcome to my webpage but you did not login yet!". Click on "try to __login here__"
9. The browser will move the login endpoint, where we need to access to continue. There are 2 accounts that was seeded before, you can use any of them:
    - account 1: username = managerTom123, password = manager1
    - account 2: username = managerJim234, password = manager2
10. When you login sucessfully, there will be 3 buttons existed: __Data Overview__, __Room Overview__, __Log Out__.
11. If you click on __Data Overview__, there will be a data table and a pie chart.
12. If you click on __Room Overview__, there will be a data table and a bar chart.
13. If you click on __Log Out__, the browser will move back to the login page.

## Activate the Dashboard with Dash and Matplotlib
14. Make sure you keep the flask api running while the Dashboard is activated.
15. Open the new terminal, type __"python dashboard.py"__ to activate the dashboard.
16. The dashboard will be opened on the Browser. There will be the dropdown list on the dashboard, which will make the bar chart change depended on what you selected.
17. When you have everything done, __ctrl+C__ on every terminal. When want to open everything again, make sure to __"flask db_drop"__ first then do everything again from 2nd step.
