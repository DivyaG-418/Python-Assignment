# Python-Assignment
#1
num = int(input("Enter a 5 digit number"))

list = []

count = 0

while num != 0:

    num = num//10
    
    count = count+1
    
for item in range(1,count+1):

    a =item * 10
    
    list.append(a)
    
    rev=list[::-1]
    
        
print(rev)

#2

s1 = input("Enter 1st String")

s2 = input("Enter 2nd String")

middle = int(len(s1) /2)

print("Original Strings are", s1, s2)

concat = s1[:middle:]+ s2 +s1[middle:]

print("After appending new string in middle", concat)


#3

s1 = input("enter a String")

s2 = s1.split()

lower = []

upper = []

for char in s1:

    if char.islower():
    
        lower+= char
        
    else:
    
        upper+= char
        
print(''.join(lower+upper))


#4

import re

r1 = "English = 78 Science = 83 Math = 68 History = 65"

markList = [int(num) for num in re.findall(r'\b\d+\b', inputStr)]

totMarks = 0

for mark in markList:

  totMarks+=mark

percent = totalMarks/len(markList)  

print("Total Marks is:", totalMarks, "Percentage is ", percentage)


#5

list1 = [3, 6, 9, 12, 15, 18, 21]

list2 = [4, 8, 12, 16, 20, 24, 28]

list3 = list()

odd = list1[1::2]

print("Element at odd-index positions from list one")

print(odd)

Even = list2[0::2]

print("Element at even-index positions from list two")

print(Even)

print("Printing Final third list")

list3.extend(odd)

list3.extend(Even)

print(list3)


