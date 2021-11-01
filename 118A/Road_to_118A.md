https://codeforces.com/problemset/problem/118/A

Overrall, we have 3 conditions
- deletes all the vowels, including A, O, Y, E, U, I
- inserts a character "." before each consonat
- replaces all uppercase consonates with lower ones
If we can identify order deploy the condtions, everything will become esaily

Note that finally, the output will be lowercase.
So let convert the input to lowercase first

After that, we move to delet all the vowels, so create a list to storage the vowels
Then use a for loop for access each character of the input. Here the logic:
- if this character belong the vowels list, nothing happens, the loop continue
- if not, add this character into the result list, so make sure you creteat a empty list to save the result first
When the loop is over, we will have a list just includ all of consonats from the input string

Finnaly, add "." for each character of the list and convert it to a string
You can use join() method to do that, like the example code. Don't forget print one more "." before the result string 