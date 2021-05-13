# Simple Django Login and Registration

An example of Django project with basic user functionality.

## Screenshots

| Log In | Create an account | Authorized page |
| -------|--------------|-----------------|
| <img src="./screenshots/login.png" width="200"> | <img src="./screenshots/create_an_account.png" width="200"> | <img src="./screenshots/authorized_page.png" width="200"> |

| Password reset | Set new password | Password change |
| ---------------|------------------|-----------------|
| <img src="./screenshots/password_reset.png" width="200"> | <img src="./screenshots/set_new_password.png" width="200"> | <img src="./screenshots/password_change.png" width="200"> |

| Session logs |
| ---------------|
| <img src="./screenshots/session_logs.png" width="200"> |

## Functionality

- Log in
    - via username & password
    - via email & password
    - via email or username & password
    - with a remember me checkbox (optional)
- Create an account
- Log out
- Profile activation via email
- Reset password
- Remind a username
- Resend an activation code
- Change password
- Change email
- Change profile
- Multilingual: English, Russian, and Simplified Chinese
- Session logs list


## Installing

### Clone the project

```
git clone https://github.com/Ramon8888/ubbitt-login-test.git
cd ubbitt-login-test
```

### Install dependencies & activate virtualenv

```
pip install pipenv

pipenv install
pipenv shell

pip install psycopg2-binary
```

### Configure the settings (connection to the database, connection to an SMTP server, and other options)

1. Edit `source/app/conf/development/settings.py` if you want to develop the project.

2. Edit `source/app/conf/production/settings.py` if you want to run the project in production.

### Create database and apply migrations

database: 'ubbitt_login'

```
python source/manage.py migrate
```

### Collect static files (only on a production server)

```
python source/manage.py collectstatic
```

### Running

#### A development server

Just run this command:

```
python source/manage.py runserver
```

#### Special thanks to 

<a href="https://github.com/egorsmkv/simple-django-login-and-register">EGORSMKV</a>

This project was based in the next repository:

```
https://github.com/egorsmkv/simple-django-login-and-register.git
```