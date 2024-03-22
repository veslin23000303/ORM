# Ex02 Django ORM Web Application
## Date:16/3/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![WhatsApp Image 2024-03-22 at 10 30 42_28ed3327](https://github.com/Veslinanish/ORM/assets/151148539/935a3a5e-9b0d-4378-a1e3-61c34c4e0f51)


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
models.py
from django.db import models
from django.contrib import admin

# Create your models here.
class Book(models.Model):
    book_id = models.IntegerField(primary_key=True)
    book_name = models.CharField(max_length=100)
    Author= models.CharField(max_length=50)
    Date= models.DateField()
    price = models.IntegerField()

class Display_book(admin.ModelAdmin):
    list_display = ('book_id','book_name','Author','Date','price')

admin.py
from django.contrib import admin
from .models import Book,Display_book
# Register your models here.

admin.site.register (Book, Display_book)
```

## OUTPUT
![Screenshot 2024-03-16 214443](https://github.com/Veslinanish/ORM/assets/163664011/43fc8a0e-3603-4a68-9353-06d420b62250)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
