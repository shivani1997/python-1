python
======

Show Me the Code Python version.

2015年8月10日更新：
【注】Pull Request 请提交你个人的仓库 URL 链接地址。

### How to Add your solutions:

  * fork this repo
  * create a folder named with your github name
  * create a folder named the problem num
  * add your solution in the folder

For example, if you wanna add a solution for problem 0001, you should do like this:

  * fork Show-Me-the-Code/python
  * git clone YOUR_REPO_URL SOME_DIR
  * cd SOME_DIR
  * mkdir YOUR_GITHUB_USER_NAME
  * cd YOU_GITHUB_USER_NAME
  * mkdir 0001
  * cd 0001
  * and the write some code & test it

if all these steps done, send us an pull request. After we accepte your request, we'll invite you to this group.

This is the simple pyton programme code:

Please note that these examples are written in Python 2, and may need some adjustment to run under Python 3.

1 line: Output

print 'Hello, world!'

2 lines: Input, assignment

name = raw_input('What is your name?\n')
print 'Hi, %s.' % name

3 lines: For loop, built-in enumerate function, new style formatting

friends = ['john', 'pat', 'gary', 'michael']
for i, name in enumerate(friends):
    print "iteration {iteration} is {name}".format(iteration=i, name=name)

4 lines: Fibonacci, tuple assignment

parents, babies = (1, 1)
while babies < 100:
    print 'This generation has {0} babies'.format(babies)
    parents, babies = (babies, parents + babies)

5 lines: Functions

def greet(name):
    print 'Hello', name
greet('Jack')
greet('Jill')
greet('Bob')

6 lines: Import, regular expressions

import re
for test_string in ['555-1212', 'ILL-EGAL']:
    if re.match(r'^\d{3}-\d{4}$', test_string):
        print test_string, 'is a valid US local phone number'
    else:
        print test_string, 'rejected'

7 lines: Dictionaries, generator expressions

prices = {'apple': 0.40, 'banana': 0.50}
my_purchase = {
    'apple': 1,
    'banana': 6}
grocery_bill = sum(prices[fruit] * my_purchase[fruit]
                   for fruit in my_purchase)
print 'I owe the grocer $%.2f' % grocery_bill

8 lines: Command line arguments, exception handling

# This program adds up integers in the command line
import sys
try:
    total = sum(int(arg) for arg in sys.argv[1:])
    print 'sum =', total
except ValueError:
    print 'Please supply integer arguments'
