# Cookie-stand-api

## Feature Tasks and Requirements
#### Use API Quick Start Template
- Create a new public repo cookie-stand-api that uses API Quick Start as a template, or use one that you have created.
- Modify your application using instructions in README.md found in root of repo.
- Install from requirements.txt.
- Export (aka freeze) requirements.
- Change things app folder to be cookie_stands
- Go through code base looking for Thing,thing and things change to cookie-stand related names.
- E.g. Thing model becomes CookieStand
- E.g. ThingList becomes CookieStandList
- Pro Tip: Do a global text search looking for thing
- Search should be case insensitive.
- WARNING: Do NOT just cut and paste. Think through each change.
- Create/rename .env using .env.sample as starting point.
- Here’s a handy way to generate a secret key
python -c “import secrets; print(secrets.token_urlsafe())”


## User:
- User: Admin
- Password: Admin

## Deployed Site:
- https://cookie-401-api.herokuapp.com/

## Customization Steps

- DO NOT migrate yet
- add additional dependencies as needed
  - Re-export requirements.txt as needed
- change `things` folder to the app name of your choice
- Search through entire code base for `Thing`,`Things` and `things` to modify code to use your resource
  - `project/settings.py`
  - `project/urls.py`
  - App's files
    - `views.py`
    - `urls.py`
    - `admin.py`
    - `serializers.py`
    - `permissions.py`
- Update ThingModel with fields you need
  - Make sure to update other modules that would be affected by Model customizations. E.g. serializers, tests, etc.
- Rename `project/.env.sample` to `.env` and update as needed
- Run makemigrations and migrate commands
- Optional: Update `api_tester.py`
