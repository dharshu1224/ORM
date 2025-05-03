# Ex02 Django ORM Web Application
## Date: 03/05/2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![Screenshot 2025-05-03 072229](https://github.com/user-attachments/assets/75c38966-c8d5-45fc-9b92-b88b2694d1ff)




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
from .models import Bankloan,BankloanAdmin
admin.site.register(Bankloan,BankloanAdmin)

models.py

from django.db import models
from django.contrib import admin
class Bankloan(models.Model):
    Name=models.CharField(max_length=50);
    Gender=models.CharField(max_length=10);
    Token_no=models.IntegerField(primary_key=True);
    Amount=models.IntegerField();
    Phone=models.IntegerField();


class BankloanAdmin(admin.ModelAdmin):
    list_display=('Name','Gender','Token_no','Amount','Phone')
```



## OUTPUT

![Screenshot 2025-05-03 072312](https://github.com/user-attachments/assets/998f5c75-4cb4-4eb9-819b-3907da772a41)



## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
