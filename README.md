# Ex02 Django ORM Web Application
## Date: 22.11.2025
## Register no:25019029

## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).


## ENTITY RELATIONSHIP DIAGRAM



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
```
----models.py
from django.db import models 
from django.contrib import admin
class amazon_DB (models.Model):
     Product_name=models.CharField(max_length=20)
     S_no=models.IntegerField (primary_key=True)
     Product_type=models.CharField(max_length=20)
     Price=models.CharField(max_length=20)
     Year=models.IntegerField()
class amazon_DBAdmin(admin.ModelAdmin):
     list_display=["Product_name","S_no","Product_type","Price","Year"]
----admin.py
from django.contrib import admin
from .models import amazon_DB,amazon_DBAdmin
admin.site.register(amazon_DB,amazon_DBAdmin)
```
##OUTPUT
<img width="1917" height="852" alt="Screenshot 2025-11-21 161245" src="https://github.com/user-attachments/assets/052d6a56-9237-43b4-b9cb-640c709aa6f4" />
<img width="1081" height="646" alt="Screenshot 2025-11-21 162036" src="https://github.com/user-attachments/assets/effeceff-1a25-48e4-b3ec-c1e9db7a9436" />


## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
