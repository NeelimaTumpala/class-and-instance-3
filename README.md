# class-and-instance-3
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
