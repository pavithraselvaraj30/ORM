# Ex02 Django ORM Web Application
## Date: 05-03-2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

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
class Books(models.Model):
      name=models.CharField(max_length=20);
      bookno=models.IntegerField(primary_key=True);

      author=models.CharField(max_length=20);
      prize=models.IntegerField();
class BooksAdmin(admin.ModelAdmin):
      list_display=("name","bookno","author","prize");


admin.py

from django.contrib import admin
from .models import Books,BooksAdmin
admin.site.register(Books,BooksAdmin)


```

## OUTPUT


![web ex](https://github.com/pavithraselvaraj30/ORM/assets/149366880/587b22b5-22c8-4672-946b-36ce06eb1b99)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
