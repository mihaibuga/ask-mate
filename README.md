<div id="top"></div>

# ASK MATE

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#main-features">Main Features</a></li>
        <li><a href="#built-with">Built With</a></li>
        <li><a href="#visuals">Visuals</a></li>
      </ul>
    </li>
    <li><a href="#installation-and-usage">Installation and Usage</a></li>
    <li><a href="#development-team">Development Team</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

Ask mate is a forum where visitors can register and login, start new discussions on different topics, respond to other topics, comment on questions and answers, and vote for answers as preffered. It's simmilar to let's say...Stack Overflow, but it's low specs version.

![home-page.png][home-page]

<p align="right">(<a href="#top">back to top</a>)</p>


### Main Features

- Register
- Login
- Sort questions
- Search key terms/phrases
- Create new question
- Answer questions
- Vote questions and answers
- Comment questions and answers
- Mark questions as selected
- Delete questions, answers and comments
- Access user dashboard
- Users statistics


<p align="right">(<a href="#top">back to top</a>)</p>

### Built With

Back End:
* [Python][python]
* [Flask][flask]

Front End:
* [HTML][html]
* [CSS][css]

Database Management:
* [PostgreSQL][postgres]

IDE:
* [Visual Studio Code][visual-studio-code]

<p align="right">(<a href="#top">back to top</a>)</p>



### Visuals

Home page:

![questions-page.png][questions-page]

Register Page:

![register-page.png][register-page]

Login Page:

![login-page.png][login-page]

Tags Page:

![tags-page.png][tags-page]

Home Page - Logged in:

![home-page-logged-in.png][home-page-logged-in]

New question Page:

![new-question-page.png][new-question-page]

New Answer Page:

![new-answer-page.png][new-answer-page]

Question Page:

![question-page.png][question-page]

User Dashboard Page:

![user-dashboard-page.png][user-dashboard-page]

Users Page:

![users-page.png][users-page]

<p align="right">(<a href="#top">back to top</a>)</p>



## Installation and Usage

### If you'd like to have a look at the application, please, follow these steps:

- Go to the [web app][heroku-app] on Heroku
- Use Demo Credentials:
	```
	user_name: nick_the_brick@yolo.com
	pass: L1nk1np@rk
	``` 
- Enjoy!

### If you'd like to edit and test the source code on Windows OS, please, follow these steps

- Install [Python][python]
- Install [PostgreSQL][postgres]
- In order to acccess the PSQL command line or python, pip, set up the environment variables with the path of the `bin` and `lib` folders of PostgreSQL directory, your Python folder path and the subfolder `Scripts`. Maybe these videos could give you a hand with this: [Set postgres path][set-postgres-env-vars], [Set python path][set-python-env-vars] 
- Install [virtualenv][virtualenv] with `pip install virtualenv` from the command prompt
- Open the root directory and create a virtual environment `virtualenv venv`
- Activate virtualenv with `venv\Scripts\activate`
- Install requirements from the `requirements.txt` `pip install -r requirements.txt`
- Install psycopg2
- Run psql
- Create a database
- Run in command line all lines from the sql file in the sample_data directory
- Run `psql -U postgres` in the command line and add the password you choose when installed PostgreSQL to login
- Create a database `psql CREATE DATABASE <DB_NAME>`
- Connect to the database you've just created `psql \c <DB_NAME>`
- Seed the database with the data from `\sample_data\askmatepart2-sample-data.sql` by using `psql \i <Copy realtive path of the askmatepart2-sample-data.sql>` change the `\` path separator with `/`
- Duplicate the `.env.template` and rename it to `.env`
- In the `.env` file fill these fields

    ```PSQL_USER_NAME=postgres account
    PSQL_PASSWORD=postgres account password
    PSQL_HOST=localhost
    PSQL_DB_NAME=db_name_you_created ```
- Run `server.py`

<p align="right">(<a href="#top">back to top</a>)</p>

## Development Team

* [Mihai Buga's GitHub][mihai-buga]
* [Nicolae Peptea's GitHub][nicolae-peptea]

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Thanks for all the support to the Codecool mentors that have guided us!


<!-- MARKDOWN LINKS & IMAGES -->
[postgres]: https://www.postgresql.org/
[python]: https://www.python.org/
[flask]: https://flask.palletsprojects.com/en/2.0.x/
[html]: https://html.com/
[css]: https://www.w3.org/Style/CSS/Overview.en.html
[visual-studio-code]: https://code.visualstudio.com/
[virtualenv]: https://pypi.org/project/virtualenv/

[mihai-buga]: https://github.com/mihaibuga
[nicolae-peptea]: https://github.com/Nicolae-Peptea

[heroku-app]:https://askmate09.herokuapp.com/

[home-page]: images/captures/home-page.png
[questions-page]: images/captures/questions-page.png
[register-page]: images/captures/register-page.png
[login-page]: images/captures/login-page.png
[tags-page]: images/captures/tags-page.png
[home-page-logged-in]: images/captures/home-page-logged-in.png
[new-question-page]: images/captures/new-question-page.png
[new-answer-page]: images/captures/new-answer-page.png
[question-page]: images/captures/question-page.png
[user-dashboard-page]: images/captures/user-dashboard-page.png
[users-page]: images/captures/users-page.png

[set-postgres-env-vars]: https://youtu.be/0CAzSXG6N8E
[set-python-env-vars]: https://youtu.be/OS5EgtMQrmQ
