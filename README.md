# Ex02 Django ORM Web Application
## Date:12.05.2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here
![Screenshot 2024-05-12 053104](https://github.com/veslin23000303/ORM/assets/151148539/154e076d-699f-41f0-9e41-b74b7eb5c3b7)



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
admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

models.py

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.IntegerField(primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
 
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')
```




## OUTPUT

Include the screenshot of your admin page.
![WhatsApp Image 2024-03-22 at 11 26 58_0f57bbb0](https://github.com/veslin23000303/ORM/assets/151148539/5fd634bf-722f-4964-bdc0-9cba6ba533d4)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully

## RELEASES
No releases published

## PACKAGES
no packages published
