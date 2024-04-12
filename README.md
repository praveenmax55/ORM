# Ex02 Django ORM Web Application
## Date: 28\02\2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![alt text](<entity relationship-1.jpeg>)

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
Name:Praveen D
Ref no. :212222240076
```

### models.py:
```
from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
      sno=models.IntegerField(primary_key="sno");
      name=models.CharField(max_length=50);
      author=models.CharField(max_length=70);
      price=models.IntegerField();
      publisher=models.CharField(max_length=60);

class Book_DBAdmin(admin.ModelAdmin):
    list_display=("sno","name","author","price","publisher");
```
 ### admin.py:
 ```
 from django.contrib import admin
 from .models import Book_DB,Book_DBAdmin
 admin.site.register(Book_DB,Book_DBAdmin)
```

## OUTPUT
![Web ex2](https://github.com/praveenmax55/ORM/assets/113497509/3c16443c-f9e2-44d0-831c-e1c85e784e98)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
