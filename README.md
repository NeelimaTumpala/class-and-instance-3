# class-and-instance-3

example 1:

class Employee:
    def __init__(self, first, last, pay):
        self.first = first
        self.last = last
        self.pay = pay
        self.email = first + '.' + last + '@company.com'

emp_1=Employee('neelima','tumpala','50000')
emp_2=Employee('jyothi','kapuganti','60000')

print(emp_1.email)
print(emp_2.email)


output:
neelima.tumpala@company.com
jyothi.kapuganti@company.com

example 2:

class Employee:
    def __init__(self, first, last, pay):
        self.first = first
        self.last = last
        self.pay = pay
        self.email = first + '.' + last + '@company.com'

emp_1=Employee('neelima','tumpala','50000')
emp_2=Employee('jyothi','kapuganti','60000')

print(emp_1.email)
print(emp_2.email)
print('{} {}'.format(emp_1.first, emp_1.last))


ouput:
neelima.tumpala@company.com
jyothi.kapuganti@company.com
neelima tumpala

example 3:

class Employee:
    def __init__(self, first, last, pay):
        self.first = first
        self.last = last
        self.pay = pay
        self.email = first + '.' + last + '@company.com'
    def fullname(self):
        return '{} {}'.format(self.first, self.last)

emp_1=Employee('neelima','tumpala','50000')
emp_2=Employee('jyothi','kapuganti','60000')

print(emp_1.email)
print(emp_2.email)
print(emp_1.fullname())
print(emp_2.fullname())

output:
neelima.tumpala@company.com
jyothi.kapuganti@company.com
neelima tumpala
jyothi kapuganti

example:

class Employee:
    def __init__(self, first, last, pay):
        self.first = first
        self.last = last
        self.pay = pay
        self.email = first + '.' + last + '@company.com'
    def fullname(self):
        return '{} {}'.format(self.first, self.last)

emp_1=Employee('neelima','tumpala','50000')
emp_2=Employee('jyothi','kapuganti','60000')

print(emp_1.email)
print(emp_2.email)
emp_1.fullname # instance
print(Employee.fullname(emp_1)) #class

output:
neelima.tumpala@company.com
jyothi.kapuganti@company.com
neelima tumpala
