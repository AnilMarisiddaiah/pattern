# pattern
this includes the some of pattern generation code in python
# 33333
# 32223
# 32123  
# 32223
# 33333
# or
#4444444
#4333334
#4322234
#4321234
#4322234
#4333334
#4444444
n = 4 # it value changes based on the number on which it has to display
for i in range(0, 2*n-1):
    for j in range(0, 2*n-1):
        for k in range(0, n):
            if k == i or k == j or i == ((2*n)-2-k) or j == ((2*n)-2-k):
                print(n - k, end="")
                break
    print()
##########################################################################
#to print the following pattern
# * * * * * * *
# * *       * *
# *   *   *   *
# *     *     *
# *   *   *   *
# * *       * *
# * * * * * * *
# n = 7 # it is based on the number n*n matrix to be displayed
# m = n
# mod = n-1
# for i in range(1, n+1):
#     for j in range(1, n+1):
#         if i % mod == 1 or j % mod == 1 or i == j or j == m:
#             print("* ", end="")
#         else:
#             print("  ", end="")
#     m = m - 1
#     print()
###########################################################
#to print the following pattern
# 1
# 232
# 45654
# 6789876
k = 4 # it is baed on the number of lines to be displayed it is better to take value to less than or equal to 4
#because after value 4 it will be printing 2 digit numbers which is annoying to see output . output is correct 
#it won't look good because of 2 digit number
var = 1
num = 0
ex = 1
for i in range(1, k+1):
    if i == 1:
        print(1, end="")
    else:
        num = num + 2
        for k in range(0, i):
            print(num, end="  ")
            num = num + 1
        num = num - 1
        for l in range(1, ex):
            num = num - 1
            print(num, end="  ")
    ex += 1
    print()
###########################################################
#to print the following pattern
# **********
# ****  ****
# ***    ***
# **      **
# *        *
x = 5 # it is based on the number of value of rows to be printed
s = 0
for i in range(0, 5):
    for j in range(0, x):
        print("*", end="")
    for k in range(0, s):
        print(" ", end="")
    for j in range(0, x):
        print("*", end="")
    print()
    x = x - 1
    s = s + 2
###########################################################
#to print the following pattern
#    *
#   *a*
#  *a*a*
# *a*a*a*
 x = 3
 ex = 1
 for i in range(0, 4):
     for k in range(0, x):
         print(" ", end="")
     for l in range(1, 2*ex):
         if l % 2 == 0:
             print("a", end="")
         else:
             print("*", end="")
     print()
     x = x - 1
     ex = ex + 1
###########################################################
#to print the following pattern
#      *
#     ***
#    *****
#   *     *
#  ***   ***
# ***** *****

k = 6 - 3 # here value 6 is based on the number of rows to be printed
sp = k*2 - 1
for i in range(1, k + 1):
    for k in range(0, sp):
        print(" ", end="")
    for j in range(1, 2*i):
        print("*", end="")
    sp -= 1
    print()
ro = 6 - 3 # here value 6 is based on the number of rows to be printed
sp = ro - 1
sp2 = ro*2
for i in range(1, ro + 1):
    for k in range(0, sp):
        print(" ", end="")
    for j in range(1, 2*i):
        print("*", end="")
    for l in range(sp2, 1, -1):
        print(" ", end="")
    for j in range(1, 2*i):
        print("*", end="")
    sp -= 1
    sp2 -= 2
    print()


