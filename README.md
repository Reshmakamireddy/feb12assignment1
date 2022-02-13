wh=300
ric=600
cht=400
swt=700
cname=input('Enter customer name :')
cphno=int(input('Enter customer phone no :'))
cfq=int(input('Enter no of cfq packets:')) 
whq=int(input('Enter no of whq packets:')) 
ricq=int(input('Enter no of ricq packets:')) 
chtq=int(input('Enter no of chtq packets :'))
swtq=int(input('Enter no of swtq packets :'))
bill=(cf*cfq)+(wh*whq)+(ric*ricq)+(cht*chtq)+(swt*swtq)
if bill>=5000:
    disc=bill*10/100
    if bill>=3000:
        disc=bill*8/100
        if bill>=2000:
            disc=bill*5/100
            if bill>=1000:
                disc=bill*3/100
    tax=0
elif bill>=3000:
    disc=bill*8/100
    tax=bill*10/100
else:
    disc=0
    tax=bill*18/100
mainbill=bill-disc+tax
print('bill amount :',mainbill)

Output:-
Enter customer name :siri
Enter customer phone no :9765432165
Enter no of cfq packets:1
Enter no of whq packets:2
Enter no of ricq packets:1
Enter no of chtq packets :1
Enter no of swtq packets :2
bill amount : 3570.0

