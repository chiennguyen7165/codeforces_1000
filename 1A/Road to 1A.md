https://codeforces.com/problemset/problem/1/A

The tast is find the minimum square granite flagstones (a x a size, fixed) to cover the rectangular (m x n size)
The area of these little rocks can be bigger than this value of the rectangular

Simplest way, you divide each side of rectangular to size of square, then rounding the result up to the nearest integer
Then multiple two resultes for the final output.
But the round() method just round by the standard way. ex 5.1 -> 5. So the approach seems not fit

Other appoarch is use the // operation - Floor division
In detail, it is a normal division operation except that it returns the largest possible integer. 
This integer is either less than or equal to the normal division result.
Ex. 15 / 4 = 3.75, so 15 // 4 = 3
The point is // will round down the reuslt so, you turn the reuslt into negativ. The result will perfectly fit
Ex. -15 / 4 = -3.75, so -15 // 4 = -4

After all, negativ x negativ = postive. So, here we final result