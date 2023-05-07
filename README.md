# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![ex 2](https://user-images.githubusercontent.com/128462891/236660168-dd95809a-c138-4f22-a1aa-bad7cac6b562.png)


Include your ER diagram here

## DESIGN STEPS

### STEP 1:

### STEP 2:

### STEP 3:

Write your own steps

## PROGRAM
```python
from django.db import models
from django.contrib import admin
class GitDatabase(models.Model):
    username_primary_key = models.CharField(max_length=30, help_text="User name must be unique", primary_key=True,unique=True)
    password = models.CharField(max_length=30)
    firstname = models.CharField(max_length=20)
    lastname = models.CharField(max_length=20)
    profile_photo = models.ImageField()
    email = models.EmailField(max_length=50,unique=True)
class GitAdmin(admin.ModelAdmin):
    list_display = ('username_primary_key', 'password', 'firstname', 'lastname','profile_photo','email')
 ```

Include your code here

## OUTPUT
(https://user-images.githubusercontent.com/121215938/233891019-d32a67de-0852-463c-b404-5fd77ece8fc2.jpg)
Include the screenshot of your admin page.


## RESULT
Thus a Danjo application is successfully developed to store and retrive data from a database using object realtion mapping

