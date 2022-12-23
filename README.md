# Blog from Lisa

Blog on Django, server part.

![](https://github.com/VAChess777/images_/blob/8e9905fc6bc9f548f7486f5d7a93468ea0494a1c/Django%20blog.png)

### Software environment and installation:

Python3 should already be installed.

### Program installation:

Download the code: [https://github.com/VAChess777/Lesson_2_Reviving_the_blog_on_Django_Layout_for_the_pitonist_Devman](https://github.com/VAChess777/Lesson_2_Reviving_the_blog_on_Django_Layout_for_the_pitonist_Devman), or clone the `git` repository to a local folder:
```
gh repo clone VAChess777/Lesson_2_Reviving_the_blog_on_Django_Layout_for_the_pitonist_Devman
```

### Installing dependencies:

Use `pip` (or `pip3`, if there is a conflict with Python2) to install dependencies:
```bach
pip install -r requirements.txt
```

### About environment variables:

The program `settings.py ` there are environment variables in the `project` folder that are responsible for configuring access to the database.
create a `.env` file, place it in the root directory of the program. Put the following data in the `.env` file in the `key=value` format.

- `DEBUG=` - True for enabling debugging mode, False for production. The default value is `False`.
- `SECRET_KEY=` - Django secret key. For example: `erofheronoirenfoernfx49389f43xf3984xf9384`.
- `DB_NAME=` - Database name.
- `ALLOWED_HOSTS=` - This is a security measure to prevent HTTP Host header attacks, which are possible even under many seemingly-safe web server configurations.
Example of ALLOWED_HOSTS settings in file. env - `ALLOWED_HOSTS = ['www.djangoproject.dev', 'docs.djangoproject.dev', 'localhost' ...]`. Where
`www.djangoproject.dev', 'docs.djangoproject.dev, 'localhost'` -  addresses of allowed hosts. The default value is `localhost`.
- `STATIC_URL` — by default, this is `'/static/'`. [What is STATIC_URL](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-STATIC_URL).
- `STATIC_ROOT` — by default, this is `'None'`, i.e. the current folder. [What is STATIC_ROOT](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-STATIC_ROOT).
- `MEDIA_URL` — by default, this is `'/media/'`. [What is MEDIA_URL](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-MEDIA_URL).
- `MEDIA_ROOT` — by default, this is `'media'`. [What is MEDIA_ROOT](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-MEDIA_ROOT).

### How to run the program:

Enter the command in console: `$ python manage.py runserver`.

### How the program works:

The program contains scripts:

```manage.py``` - the program that runs the server.               
```settings.py``` - the program is located in the project folder. Responsible for setting up access to the database.                    
```models.py``` - the program is located in the datacenter folder. The program is responsible for data models and their fields.                    
```urls.py``` - the program is located in the project folder. Responsible for setting up links to blog pages.                    

### Project Goals

This code was written for educational purposes as part of an online course for web developers at [dvmn.org](https://dvmn.org/).
