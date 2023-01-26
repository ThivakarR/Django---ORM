# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![image](https://user-images.githubusercontent.com/118348224/211608369-3e1ba8b6-2ae3-44d5-80ea-2e2e32d00a3b.png)

## DESIGN STEPS

### STEP 1:
creating a table using required details in Django--ORM.
### STEP 2:
Upload the python code.
### STEP 3:
push the code to github.
## PROGRAM
```
admin.py:

from django.contrib import admin
from .models import Student,StudentAdmin


admin.site.register(Student,StudentAdmin)

manage.py:

from django.db import models
from django.contrib import admin
# Create your models here.

class Student(models.Model):
    referencenumber=models.CharField(max_length=10,help_text="Your Reference Number")
    name=models.CharField(max_length=100)
    department=models.CharField(max_length=200)
    age=models.IntegerField()
    email=models.EmailField()

class StudentAdmin(admin.ModelAdmin):
    list_display = ('referencenumber','name','age','department','email')
# Register your models here.
```
## OUTPUT

![dj](https://user-images.githubusercontent.com/118707074/214840224-9f0392bd-d09f-4a47-960e-89562a30ca84.png)



## RESULT

Thus, the experiment was executed successfully..
