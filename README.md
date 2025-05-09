#for wiyh in range
n=int(input("enter the vaue of n"))
for i in range(10,n+1,-1):
    print(i,end='  ')
for i in range(n,0,-2):
    print(i,end=' ')
output:
enter the vaue of n 5
10  9  8  7  5 3 1 

#multiplication
n=int(input("enter n"))
for i in range(1,11):
    print(f"{n} X {i} = {n*i}")
output:
12 X 1 = 12
12 X 2 = 24
12 X 3 = 36
12 X 4 = 48
12 X 5 = 60
12 X 6 = 72
12 X 7 = 84
12 X 8 = 96
12 X 9 = 108
12 X 10 = 120

#all the leap years from 1900 to 2101
st=int(input("enter start year"))
en=int(input("enter end year"))
for i in range(st,en+1):
    if i%4==0:
        print(i,end=' ')  
output:
enter start year 1900
enter end year 2101
1900 1904 1908 1912 1916 1920 1924 1928 1932 1936 1940 1944 1948 1952 1956 1960 1964 1968 1972 1976 1980 1984 1988 1992 1996 2000 2004 2008 2012 2016 2020 2024 2028 2032 2036 2040 2044 2048 2052 2056 2060 2064 2068 2072 2076 2080 2084 2088 2092 2096 2100 

#sum of series in form 1/n^2
n=int(input("enter the value of n "))
s=0
for i in range(1,n+1):
    a=1/(i**2)
    s+=a
print(s)
OUTPUT:
enter the value of n  5
1.4636111111111112

#sum of series in form n^n/n
n=int(input("enter the value of n "))
s=0
for i in range(1,n+1):
    a=(i**i)/i
    s+=a
print(s)
OUTPUT:
enter the value of n  5
701.0

#generating a manual calendar
stday=int(input("enter starting day of month(1-7)"))
ndays=int(input("enter number of days in the month"))
print("sun mon tue wed thu fri sat")
print("***************************")
for i in range(stday-1):
    print(end="   ")
i=stday-1
for j in range(1,ndays+1):
    if i>6:
        print()
        i=1
    else:
        i+=1
    print(str(j)+" ",end=' ')
OUTPUT:








#generating a manual calendar
stday=int(input("enter starting day of month(1-7)"))
ndays=int(input("enter number of days in the month"))
print("sun mon tue wed thu fri sat")
print("***************************")
for i in range(stday-1):
    print(end="   ")
i=stday-1
for j in range(1,ndays+1):
    if i>6:
        print()
        i=1
    else:
        i+=1
    print(str(j)+" ",end=' ')

enter starting day of month(1-7) 1
enter number of days in the month 31
sun mon tue wed thu fri sat
***************************
1   2   3   4   5   6    7  
8   9   10  11  12  13  14  
15  16  17  18  19  20  21  
22  23  24  25  26  27  28  
29  30  31  

#calander progrm
mdays=31
sdays=2

print("sun  mon tue wed thu fri sat")
for _ in range(sday):
    print("   ",end=' ')
for days in range(1,mdays+1):
    print(f"{days:>3}",end=' ')
    if(sdays+days)%7==0:
        print()
OUTPUT:
sun  mon tue wed thu fri sat
          1   2   3   4   5 
  6   7   8   9  10  11  12 
 13  14  15  16  17  18  19 
 20  21  22  23  24  25  26 
 27  28  29  30  31 
