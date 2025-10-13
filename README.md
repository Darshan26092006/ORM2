# Ex02 Django ORM Web Application
## Date: 13-10-2025

## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![WhatsApp Image 2025-09-25 at 21 54 11_b42e62d9](https://github.com/user-attachments/assets/67ca3d20-c898-4989-aaa5-db1983234675)



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
model.py
from django.db import models
from django.contrib import admin

class Car(models.Model):
    id = models.IntegerField(primary_key=True)
    brand = models.CharField(max_length=15)
    model = models.CharField(max_length=30)
    year = models.DateField()
    price = models.IntegerField()

class CarAdmin(admin.ModelAdmin):
    list_display = ('id','brand','model','year','price')
```

```
admin.py
from django.contrib import admin
from . models import Car, CarAdmin

# Register your models here.
admin.site.register(Car, CarAdmin)
```


## OUTPUT

<img width="1919" height="982" alt="image" src="https://github.com/user-attachments/assets/772d40ba-911b-4f72-a167-06a9ea4d93b7" />


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
