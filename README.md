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
      bookid=models.IntegerField();
      author=models.CharField(max_length=20);
      prize=models.IntegerField();
class BooksAdmin(admin.ModelAdmin):
      list_display=("name","bookno","author","prize","bookid");


admin.py

from django.contrib import admin
from .models import Books,BooksAdmin
admin.site.register(Books,BooksAdmin)


```

## OUTPUT


![mind map](https://github.com/pavithraselvaraj30/ORM/assets/149366880/5c6c49de-4400-43e6-aa3d-3ac3bac1454d)


![Screenshot 2024-04-04 205432](https://github.com/pavithraselvaraj30/ORM/assets/149366880/d72af30b-7704-482b-8ea4-74b6ed59436f)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
