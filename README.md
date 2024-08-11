# if-else-alif
#1
age=2
if age>=18:
    print("you are adult")
    print("you can vote")
elif age<18 and age>3:
    print("you are in school")
else:
    print("you are a kid")
print('thanks')

#2
first=int(input("enter 1st number :"))
operator=input("enter operator: (+,-,*,/,%)")
second=int(input("enter second number : "))
if operator=='+':
    print(first+second)
elif operator=='-':
    print(first-second)
elif operator=='*':
    print(first*second)
elif operator=='/':
    print(first/second)
elif operator=='%':
    print(first%second)
else:
    print("invalid")



#3
s=str(input("enter a sentence : "))
for chr in s:
    if chr=='A' or chr=='a':
        print("vowel 'a' is present")
    elif chr=='E' or chr=='e':
        print("vowel 'e' is present")
    elif chr=='I'or chr=='i':
        print("vowel 'i' is present")
    elif chr=="O" or chr=="o":
        print("vowel 'o' is present")
    elif chr=="U" or chr=="u":
        print("vowel 'u' is present")

#4
t1=0
t2=1
terms=int(input("how many terms do you want : "))
t=1
while t<=terms:
    if t==1:
        print(t1," , ",end=" ")
        t+=1
        continue 
    if t==2:
        print(t2," , ",end=" ")
        t+=1
        continue
    nextTerm=t1+t2
    print(nextTerm," , ",end=" ")
    t1=t2
    t2=nextTerm
    t+=1

    
#5
n=int(input("enter the number of terms : "))
t1=0
t2=1
count=0
if n<=0:
    print("invalid input,please enter a positive integer : ")
elif n==1:
    print("fibonocii series upto",n,":")
    print(t1)
else:
    print('fibonocii sequence : ')
    while count<n:
        print(t1)
        nth=t1+t2
        t1=t2
        t2=nth
        count+=1
