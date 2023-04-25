# Hierarchical-Inheritance
class Employee:
    def __init__(self,name,employee_id,salary):
        self.name=name
        self.employee_id=employee_id
        self.salary=salary
        
    
    def display(self):
        print('name:',self.name)
        print('employee_id:',self.employee_id)
        print('salary:',self.salary)
       
    
class Manager(Employee):
    
    def __init__(self,name,employee_id,salary,team_members):
        super().__init__(name,employee_id,salary)
        self.team_members=team_members
        
    def display(self):  
        super().display()
        print('team members:',self.team_members)
        
class Teamleader(Employee):
    def __init__(self,name,employee_id,salary,team_members2):
        super().__init__(name,employee_id,salary)
        self.team_members2=team_members2
        
    def disp(self):
        super().display()
        print('team members:',self.team_members2)
        
        
obj=Manager('saksham','umpopop',150000,'sagar,yash,shubham')
print(obj.display())
obj1=Teamleader('anurag','umpocut',120000,'ujjwal_sunny_shrey')
print(obj1.disp())
    
