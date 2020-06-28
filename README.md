# Abstract_Class
to code in oop in python
from abc import ABC, abstractmethod 
class Car(ABC):
        def model(self):
            pass
        def color(self):
            pass
        def price(self):
            pass
class Car1(Car):
    def model(self,model):
        self.model=model
        print('This car model is:',self.model)
    def color(self,color):
        self.color=color
        print('This car color is.',self.color)    
    def price(self,price):
        self.price=price
        print('This car price is',self.price)
class Car2(Car):
    def model(self,model):
        self.model=model
        print('This car model is:',self.model)
    def color(self,color):
        self.color=color
        print('This car color is.',self.color)
    def price(self,price):
        self.price=price
        print('This car price is',self.price)    
        S=Car1()
S.model('Mehran')
S.color('white')
S.price(250000)
Z=Car2()
Z.model('Carolla')
Z.color('Black')
Z.price(8000000)



from abc import ABC, abstractmethod 
class Bank(ABC):
    def AccountName(self):
        pass
    def deposite(self):
        pass
    def withdraw(self): 
        pass
    
class Customer(Bank):
    def AccountName(self,name):
        self.name=name
        print('This ACCOUNT NAME IS:',self.name)
    def deposite(self,name,deposite_amount):
        self.name=name
        self.deposite_amount=deposite_amount
        print(self.name,'has deposite',self.deposite_amount,'from his account')
    def withdraw(self,name,withdraw_amount): 
        self.name=name
        self.withdraw_amount=withdraw_amount
        print(self.name,self.withdraw_amount)
        
class Customer1(Bank):  
    def AccountName(self,name):
        self.name=name
        print('This ACCOUNT NAME IS:',self.name)
    def deposite(self,name,deposite_amount):
        self.name=name
        self.deposite_amount=deposite_amount
        print(self.name,'has deposite',self.deposite_amount,'from his account')
    def withdraw(self,name,withdraw_amount): 
        self.name=name
        self.withdraw_amount=withdraw_amount
        print(self.name,self.withdraw_amount)
A=Customer()   
A.AccountName('Mian Ather Ali')
A.deposite('Ather Ali',12500000)
A.withdraw('Ather Ali',5000000)
B=Customer1()   
B.AccountName('Siraj Ahmed')
B.deposite('Siraj Ahmed',12500000)
B.withdraw('Siraj Ahmed',100000)
