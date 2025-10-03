# Python - Flask - Setup Project

A flexible, organized, and clean Python 3.10 project structure ready for implementing new projects with Conda.



## Conda Snippets

### Create environment
``` conda env create -n pfsp-env -f ./env.yml ```

### Update environment
``` conda env update -n pfsp-env -f ./env.yml ```

### Remove environment
``` conda env remove --n pfsp-setup-env ```

### List environment
``` conda env list ```

### Activate environment
``` conda activate pfsp-env ```

### Deactivate environment
``` conda deactivate ```



## To Execute

## Create '.env' file

```
SECRET_KEY="super-secret-key"
SQLALCHEMY_DATABASE_URI="sqlite:///db.sqlite"
```

### Config the DB
```
flask db init
flask db migrate -m "initial migration"
flask db upgrade
flask db downgrade
```

### Run Flask server
``` flask run ```

### Run uvicorn server (prod)
``` uvicorn src.main:asgi_app --host 0.0.0.0 --port 8000 --workers 4 --reload ```

## Links

[github_author](https://github.com/Diegoomal)

[generate-token](https://github.com/settings/tokens)
[freecodecamp-tutorial](https://www.freecodecamp.org/news/how-to-authenticate-users-in-flask/)
[digitalocean-migration-tutorial](https://www.digitalocean.com/community/tutorials/how-to-perform-flask-sqlalchemy-migrations-using-flask-migrate)

<!-- 
flask db upgrade OR downgrade
path -> migrations/script.py.mako
-->
