# Create-ER-Diagram-for-Django-Project-automatically
This Repo includes a pdf of how to create ER Diagram automatically for Django project.<br><br>
Steps to generate ER Diagram for Django App:
1. Install Graphviz software in your laptop
https://www.graphviz.org/download/
While installing add this to your system path.
or
2. pip install graphviz
Perform any one step either 1 or 2 depending on your OS.
For windows step 1 works fine.
3. pip install django-extensions
4. Go to settings.py > add 'django_extensions', to INSTALLED_APPS
5. Add the following code 
GRAPH_MODELS ={
    'all_applications': True,
    'graph_models': True,
     }
 to settings.py
6. pip install pyparsing pydot
7. python manage.py graph_models -a > erd.dot
8. python manage.py graph_models -a
9. python manage.py graph_models -a > erd.dot && python manage.py graph_models --pydot -a -g -o erd.png

