# Hackerearth-Problem
Problem
You are required to enter a word that consists of x and y that denote the number of Zs and Os respectively. The input word is considered similar to word zoo if 2*x=y.

Determine if the entered word is similar to word zoo.

For example, words such as zzoooo and zzzoooooo are similar to word zoo but not the words such as zzooo and zzzooooo.

Input format

First line: A word that starts with several Zs and continues by several Os.
Note: The maximum length of this word must be .


Output format

Print Yes if the input word can be considered as the string zoo otherwise, print No.



//////python code /////

string=input( )
string2='zoo'

s2=''
s1=''
for i in range(0,len(string)):
  if string[i]=='z':
    s1+='z'
    i=i+1


for j in range(0,len(string)):
  if string[j] =='o':
    s2+='o'
    j+=1


c2=len(s2)%len(s1)


while len(string)<20:
    if len(s2)==len(s1):
        print("No")
        break
    if c2==0:

        print("Yes") 
        break  
    else:
        print("No") 
        break
