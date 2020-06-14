# SurveyBobby  
  
In this team project, I individually was responsible for the user and admin dashboard, both interface design and implementation. Together with my teammates we developed a structure for database, and wrote our own SQL queries to power our individual pages. In addition, I designed and coded the footer section, which was common for almost all pages of the website. One of the biggest challenges, on top of learning PHP syntax (since this was our first ever PHP project), was database interaction. We wanted to structure the database in a way that it had no redundancy: same information did not appear in several tables, and in general to have as few tables, as possible. We were able to achieve this by including foreign keys in some tables, to be able to join effectively join two ore more tables when we need to retrieve data. 

**__Team: Curious Raccoons__**  

Hilmi Yildirim, Michael Pavlovic (@MichaelPavlovic), Mounica Sykam (@MounicaSykam), Vitaliy Bulyma (@VitaliyBulyma)
  
## :white_check_mark: Project Description  
  
The purpose of the website is to allow registered users to create their own surveys, and make them available for other registered users to fill. The survey creators input the Title, short description, and select category. Next, they input their questions that will appear on the surveys. Answer options to the surveys’ questions are standard for all surveys and autogenerated by the website, they are: “Strongly Disagree”, “Disagree”, “Neutral”, “Agree”, “Strongly Agree”. This structure will allow us to use algorithms to analyse customer satisfaction, or participation level (depending on the category) on a scale from 1 to 5.   The creators of the surveys will be able to see how many times the survey was filled by others, and see on the grade from 1 to 5 the average score amongst all survey results. 
Unregistered users will only be able to see the main/home page where they will find our logo, “Register” and “Login” buttons, information about our website and how it works, FAQs, and our contact information. In addition, they will see one “sample survey” accessible from the top navigation bar to give an idea how the survey looks like.

Registered users will be able to Log-in on the main page, and will be re-directed to their User Dashboard, where they will see a list of all surveys that they have created, and statistic associated with each survey. They will be able to follow the link to create new surveys from their dashboard.  As well as, able to go to the main page where, as registered users, they will see a list of all surveys available, and select one to fill if desire. In addition, from their dashboard they will be able to update their own profile, and even delete the account. 

Administrator following the Login will be re-directed to the Admin Dashboard, where they will be able to see “At Glance” information about all users in a system, and users registered in a last 30 days. Similarly, surveys information will be displayed including total surveys, and surveys created in a last 30 days. Also, administrator is able to see list of all surveys, where they will be able to remove them, and a list of all users registered with an option to delete the user form the system. From Admin dashboard, administrator will be able to access home page management page.

  
The project demo is live here: http://knx.jmn.mybluehost.me/curiousraccoons  
  
**Dependencies:** To run the project locally, clone the repository and run it on the local host. You also need to setup a local database with the name "surveybobby" and the "surveybobby.sql" file you can find in "sql" folder.   
  
## :arrow_forward: How it works 
  
The introductory information and the frequently asked questions can be found on the home page. When you are ready, just hit the "Register" button:  
  
![Home Page](/ss/home.png)
  
### Create a user or login  
  
Register with your email address and it's your username. After registering, you will be redirected to the login page.  
  
<img src="/ss/register.png" alt="Register" width="600">  
  
### User DashBoard  
  
User dashboard shows the basic profile info, the surveys created and the surveys taken. Press the "Create New Survey" button to create a new one.  
  
<img src="/ss/udash.png" alt="User Dashboard" width="800">  
  
### Create a Survey  
  
To create a survey, enter the survey title and description. After selecting a pre-defined category, you are ready to go. (categories in the drop down is being displayed by getting them from tht Surveys table)
  
<img src="/ss/create.png" alt="Create Survey" width="600">  
  
### Add Questions to a survey  
  
You can add questions to the survey on the survey details page. 
  
<img src="/ss/survey.png" alt="Add Questions" width="600">  
  
### See all surveys  
  
On the user dashboard, click "All Surveys" and you can see all available surveys.  
  
<img src="/ss/all.png" alt="Survey List" width="800">  
  
### Take a survey  
  
Select a survey on the list and press "Take Survey" button. Now, you can take the survey and submit your responses.  
  
<img src="/ss/take.png" alt="Take Survey" width="600">  
  
### Admin Dashboard  
  
You can see the admins' functionalities on the admin dashboard page when logged in with an admin account.  
  
<img src="/ss/adash.png" alt="Take Survey" width="800">  
  
## :key: Sample Credentials  
  
You can use these credentials to test the website.  
  
| Email Address | Password | isAdmin |
| ------------- |:-------------:| -----:|
| petergriffin@gmail.com | pumpkin | yes |
| cbing@gmail.com | friends| no |
| bobd@gmail.com | password | no |
 
## :globe_with_meridians: Teamwork  
  
Team members and their contributions are listed below.  
  
#### N01375163: Hilmi Yildirim  
  
- Implemented SignIn, SignUp (CRUD for `users`) and TakeSurvey pages  
- Deployed the website to the server and connected the database
- Hashed passwords, Wrote readMe, ...
  
#### N01401486: Michael Pavlovic  
  
- Implemented the home and the manageHome pages (CRUD for `faq`, `explanations`)  
- Developed CRUD for `questions` and the update functionality for `surveys`  
- Coded the sessions, the header for the logged in users, ...
  
#### N01363730: Mounica Sykam 
  
- Implemented CRUD for `categories`  
- Coded adding `surveys` and `questions`  
- Coded for listing the surveys
- Created Survey statistics page
- Developed the main header, contributed to the Survey class, ...
  
#### N00224782: Vitaliy Bulyma   

- Implemented the user and admin dashboards
- Developed the User class and contributed to `users` CRUD  
- Coded the footer, tested the website, ...


