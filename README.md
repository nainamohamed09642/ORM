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
from django.db import models
from django.contrib import admin

class Bankloan(models.Model):
    customerid= models.IntegerField(primary_key=True)
    customerrate = models.IntegerField()
    age = models.IntegerField()  
    cust_no = models.IntegerField()
    customerloan_purpose =models.CharField(max_length=500)

class BankloanAdmin(admin.ModelAdmin):
    list_display = ('customerid', 'customerrate', 'age', 'cust_no', 'customerloan_purpose')
Admin.py

from django.contrib import admin
from .models import Bankloan, BankloanAdmin  
admin.site.register(Bankloan, BankloanAdmin)
## OUTPUT
Include the screenshot of your admin page.
![Screenshot 2024-10-03 114208](https://github.com/user-attachments/assets/bb40bbfb-43f3-403c-8015-eca9b85a19e9)

## ENTITY RELATIONSHIP DIAGRAM:
![Screenshot 2024-10-03 115057](https://github.com/user-attachments/assets/03bf4452-c954-4260-972a-8e57db2dac8e)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
