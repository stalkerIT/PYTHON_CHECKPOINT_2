# PYTHON_CHECKPOINT_2
#First question 
number=[]
for x in range(2000, 3201):
    if (x%7==0) and (x%5>0):
        number.append(str(x))
print (','.join(number))
# OUTPUT:
2002,2009,2016,2023,2037,2044,2051,2058,2072,2079,2086,2093,2107,2114,2121,2128,2142,2149,2156,2163,2177,2184,2191,2198,2212,2219,2226,2233,2247,2254,2261,2268,2282,2289,2296,2303,2317,2324,2331,2338,2352,2359,2366,2373,2387,2394,2401,2408,2422,2429,2436,2443,2457,2464,2471,2478,2492,2499,2506,2513,2527,2534,2541,2548,2562,2569,2576,2583,2597,2604,2611,2618,2632,2639,2646,2653,2667,2674,2681,2688,2702,2709,2716,2723,2737,2744,2751,2758,2772,2779,2786,2793,2807,2814,2821,2828,2842,2849,2856,2863,2877,2884,2891,2898,2912,2919,2926,2933,2947,2954,2961,2968,2982,2989,2996,3003,3017,3024,3031,3038,3052,3059,3066,3073,3087,3094,3101,3108,3122,3129,3136,3143,3157,3164,3171,3178,3192,3199


#Second question
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)
n=int(input("Input a number to compute the factiorial : "))
print(factorial(n))
# OUTPUT :
Input a number to compute the factiorial : 4
24


# Third question 
number = int(input("Type a number: "))
numberDict = {}
for i in range(1, number+1):
 numberDict[i] = i*i
print(numberDict)
#OUTPUT :
Type a number: 4
{1: 1, 2: 4, 3: 9, 4: 16}

# Fourth question 

def remove_char(str, n):
      first_part = str[:n] 
      last_part = str[n+1:]
      return first_part + last_part
print(remove_char('Python', 0))
print(remove_char('Python', 4))
print(remove_char('Python', 2))

# OUTPUT :
ython
Pythn
Pyhon


# Fifth question 
import numpy as np
x= np.arange(6).reshape(3, 2)
print("Original array elements:")
print(x)
print("Array to list:")
print(x.tolist())

# OUTPUT :
Original array elements:
[[0 1]
 [2 3]
 [4 5]]
Array to list:
[[0, 1], [2, 3], [4, 5]]


# Sixth question 

x = [0, 1,  2]
>>> y = [2,  1,  0]
>>> X = np.stack((x, y), axis=0)
>>> np.cov(X)
np.cov(x,y)

#OUTPUT:
array([[ 1., -1.],
       [-1.,  1.]])
       
       
# Seventh question 

import math

numbers = input("Provide D: ")
numbers = numbers.split(',')

result_list = []
for D in numbers:
    Q = round(math.sqrt(2 * 50 * int(D) / 30))
    result_list.append(Q)

print(result_list)

#output :
Provide D: 34
[11]
