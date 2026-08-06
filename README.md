# Learning-Django
from today 1 august 2026, i started to learn django for backend services.

# installation setup :-
before installation some setup required as well 
1. pip install uv
2. uv venv
3. venv/scripts/activate
4. uv pip install Django

starts django projects command :- django-admin startproject chaiaurDjango

# files levels 
1. project levels - file name level
2. Root levels - manage.py ~ after installation this file visible
3. settings.py - Django details -> helpful in Production works
4. url.py - needs in Routing
5. views - Business logic (url.py -> route handle -> views)
6. models.py - databases connections (sqlite file name -> connects -> every knowned database)
# Django request to response data flows  ~ "MVT architecture"

"user -> request -> urls .py -> views .py -> models .py -> DB (or/) views .py -> response -> templates" 
1. Response -> views.py
2. Render -> templates folder by views.py
3. Template Engine -> Inject Programatical code and add code in html by code injecting.
4. Folders -> files
   (i). templates -> index.html
  (ii). static -> style.css, scripts.js

# Jinja2 and Django app connected 
1. jinja2 -> Django template language
2. We generally use default  templates in django.
3. if new templates use then easy define into settings .py 
4. here we use  chai .py
5. CookedInfiles > files by django

# Tailwind and admin panel setup 
1. pip install django-tailwind > add tailwind app name > runserver > tailwind runserver > setting.py > add NPM_BIN_PATH = r"D:\program files\etc\etc"
2. django_browser_reload -> add into installed apps of setting.py > (to avoid reloading)
3. add "django_browser_reload" links into middleware of settings.py > (from documentation)
4. add django_browser_related path to url.py > (put at very last helps in production time to remove it lastly)
5. migration -> we can't directly talk to databases but django can using "ORM" to talk to database.
6. migration allows admin panel and its userID password addition.
7. migration 2 commands are:-
8. i. python manage.py migrate > then add /admin after url address. > (for admin panel)
9. ii. python manage.py createsuperuser > (for ID and password)
10. lastly -> python manage.py runserver > (localhost link open)
11. Django is a "batteries-included" Python web framework > provides a complete collection of built-in tools and modules right out of the box.

# Database Connectivity and Migrations and admin panel interaction 
1. Database should be in  sepreate file - helps in production
2. no interaction to DB -> write on models.py -> it runs sql query in background.
3. model.py(in app file) -> add all DB constraints -> settings.py (edit in root folder) -> url.py (add links settings, static, others....)
4. Migrations - manually tells by django to databases about changes to load files -> "python manage.py makemigrations app_folder_name" & "python manage.py migrate"
5. admin.py - inside it attach or add models -> from .models import ChaiVarity & admin.site.register(ChaiVarity)
6. views.py -> Database details visible to frontend part template
7. added description field in database -> models.py - description = model. etc... -> migrate in database make migrations then migrate -> runserver
8. ORM - no sql query required only what to do in model.py in python.
9. {} - variables
10. % % - templates 
