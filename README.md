# Ex02 Django ORM Web Application
# Date:14/10/2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
admin.py

from django.contrib import admin 
from.models import Loan,LoanAdmin
admin.site.register(Loan,LoanAdmin)

models.py

from django.db import models
from django.contrib import admin
class Loan(models.Model):
        Name=models.CharField(max_length=10)
        Accountno=models.IntegerField(primary_key="Refno")
        Address=models.CharField(max_length=30)
        Aadharno=models.IntegerField()
        Email=models.EmailField()
class LoanAdmin(admin.ModelAdmin):
         list_display=('Name','Accountno','Address','Aadharno','Email')
```
# OUTPUT
![Screenshot 2024-12-07 231547](https://github.com/user-attachments/assets/041f81fc-d03b-44d2-bc41-792b2e01bddd)
![Screenshot 2024-12-07 231557](https://github.com/user-attachments/assets/c73b2f17-7340-449e-a75a-7754c1eeef8f)
![Screenshot 2024-12-07 231731](https://github.com/user-attachments/assets/1048033f-18a1-4348-9f60-e0869b96e02d)




# RESULT
Thus the program for creating a database using ORM hass been executed successfully
