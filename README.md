# Ex02 Django ORM Web Application
## Date: 22.04.2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![image](https://github.com/user-attachments/assets/cd2e8587-3180-4c8d-b8bf-ff7d815502ec)


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
from .models import Movie_DB,Movie_DBAdmin 
admin.site.register(Movie_DB,Movie_DBAdmin)

models.py

from django.db import models 
from django.contrib import admin 
class  Movie_DB(models.Model): 
    Movie_ID = models.CharField(max_length=20, primary_key=True) 
    Title = models.CharField(max_length=100) 
    Genre = models.CharField(max_length=20) 
    Rating = models.IntegerField( ) 
    Language = models.CharField(max_length=15) 
    Release_Date = models.DateField( ) 

class Movie_DBAdmin(admin.ModelAdmin): 
    list_display = ('Movie_ID', 'Title', 'Genre', 'Rating', 'Language', 'Release_Date') 
```

## OUTPUT

![Screenshot 2025-04-22 083802](https://github.com/user-attachments/assets/51b904e1-020f-46d5-b379-8798fc75abc4)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
