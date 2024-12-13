# Ex02 Django ORM Web Application
# Date: 20.09.2024

# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).


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
from .models import BankLoan,BankLoanAdmin
admin.site.register(BankLoan,BankLoanAdmin)

models.py

from django.db import models
from django.contrib import admin 
class BankLoan(models.Model):
  acc=models.IntegerField(primary_key="accno")
  ph=models.IntegerField()
  ifsc=models.CharField(max_length=100)
  loanno=models.IntegerField()
  adress=models.CharField(max_length=100)
  pan=models.IntegerField()
  adhar=models.IntegerField()

class BankLoanAdmin(admin.ModelAdmin):
 list_display=('acc','ph','ifsc','loanno','adress','pan','adhar',)
```

# OUTPUT
![IMG-20241213-WA0016 1](https://github.com/user-attachments/assets/50782bed-7549-4866-9e80-39ddcdc55699)

![Screenshot (85)](https://github.com/user-attachments/assets/954486e2-01e9-48e7-b703-7de6587438d8)

# ER DIAGRAM
![BANK LOAN 1](https://github.com/user-attachments/assets/8edbbdf6-4056-40e9-a701-228d955244e7)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
