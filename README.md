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
   i. templates -> index.html
  ii. static -> style.css, scripts.py 
