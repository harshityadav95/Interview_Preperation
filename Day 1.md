# Day 1 Code Tutorial and Lessons :

### Problem 1 : Source : http://hr.gs/eq5 

Key Takeaway : (Sorting Nested List)

```
main.sort(key=lambda x:x[1]) 
```


### Problem 2 : Source : https://leetcode.com/problems/reverse-integer/

Key Takeaway : Finding if a number is in range of int32 [2^31 ,2^31-1]

Solution in Python : [Can Hardcode the values of 2^31 for O(1) time limit]

```
class Solution:
    def reverse(self, x: int) -> int:
        flag=0
        if x<0:
            flag=1
            x=abs(x)
        a=0
        while(x!=0):
            a=a*10+(x%10)
            x=x//10
        if flag==1:
            a=a*-1
        if(a<(-2**31) or a>((2**31)-1)):
            return 0
        else:
  
            return a
 ```
 -- In C++ compare with INT_MAX or INT_MIN
