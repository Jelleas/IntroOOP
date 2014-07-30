IntroOOP
========

Lets say we want to write a program that models your bankaccount. We want to be able to model deposit and withdraw. This can be done as follows by introducing a global variable say bank_account, and some functions that operate on this bankaccount. For instance:

    bank_account = 1000.0
    
    def deposit(bank_account, amount):
        return bank_account + amount
        
    def withdraw(bank_account, amount):
        return bank_account - amount
        
However these two functions are designed for a bankaccount. They should only operate on bankaccounts, yet in the scope of a larger program this isn't immediately clear. By now you've already used methods of for instance strings with the dot syntax. For instance:

    print "HeLlO".lower()
    
We can achieve the same syntax for our bankaccount program by introducing objects. However, you've already worked with objects. For instance a string is an object. An object is just a concept, a way of thinking about a part of your program. For our program we could use a bankaccount object, so an object that models a bankaccount, similarly as a string object models a string. However there's no bankaccount object by default in Python because why would there be? So we need to introduce our own. To do this we need to create a class as follows:

    class Bank_account:
        pass
        
By doing this we create a new type called Bank\_account, so now not only do we have Integers, Strings, Floats etc. but also a Bank\_account. The word pass does what you think it does, it passes, so essentially does nothing. It needs to be there as whenever you open a block in Python, Python expects it to have a body, which in this case is just pass. Now we have the type Bank\_account we can create an object or otherwise called instance of this class:

    bank_account = Bank_account()
    
However, 
