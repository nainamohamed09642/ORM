# EX 02 Django ORM Web Application
## Date: 26.09.24
## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
Models.py

from django.db import models
from django.contrib import admin
class Players(models.Model):
    jrsy=models.CharField(max_length=20,help_text="Player Jrsy")
    name=models.CharField(max_length=100)
    cntry=models.CharField(max_length=100)
    age=models.IntegerField()
    height=models.IntegerField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('jrsy','name','cntry','age','height')


Admin.py

from django.contrib import admin
from .models import Players,EmployeeAdmin
admin.site.register(Players,EmployeeAdmin)
## OUTPUT
Include the screenshot of your admin page.
![image](https://github.com/230131249/ORM/assets/150232701/438dd236-4c07-4c88-89c5-86328b5acf17)
![image](https://github.com/user-attachments/assets/30beafb8-1b4a-4af6-b27f-2bc0bc063e3d)
## ENTITY RELATIONSHIP DIAGRAM:
![image](https://github.com/user-attachments/assets/b045cb10-481f-4ae1-a1c8-449cb0f30676)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
