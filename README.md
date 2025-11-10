# Ex02 Django ORM Web Application
## Date: 10.11.2025

## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![WhatsApp Image 2025-09-13 at 11 18 52_5d24c06f](https://github.com/user-attachments/assets/b5d38720-f6cf-434b-ad7b-5601ec63a6a2)


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
## Manage.py
```python
from django.db import models

# Create your models here.
class Car(models.Model):
    car_id = models.IntegerField(primary_key=True)
    brand = models.CharField(max_length=20)
    model = models.CharField(max_length=20)
    price = models.IntegerField()
    year = models.DateField()
```

## Admin.py

```python
from django.contrib import admin
from . models import Car

admin.site.register(Car)
class carAdmin(admin.ModelAdmin):
    list_display = ('car_id','brand','model','price','year')

```


## OUTPUT
<img width="1920" height="1080" alt="Screenshot 2025-09-22 085715" src="https://github.com/user-attachments/assets/235280a3-a664-4658-a6a6-58112c44246e" />



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
