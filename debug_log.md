# Debug Log

**Explain how you used the VSCode debugger tools to uncover the bugs in Exercise 7. Be specific. What breakpoints did you set? Where did you step to? What made you realize the error?**

_Example: I set a breakpoint on line 5 and stepped until line 12. There, I discovered that the `x` variable had a value of `-3`, whereas it should have had a value of `7`. That made me realize that we should be adding the two numbers `x` and `y`, instead of subtracting._

[[Your answer goes here!]]


## Exercise 5 

When it hits the if statment (if list_of_nums[i] > list_of_nums[i+1])
I get an IndexError : list index out of range
When looking at the variables tab, I see i = 5 and the len of list of nums is 6 which doesn't exist. So i need to stop the loop one iteration before. So I added the -1 in the for loop so we don't loop to far. 

## Exercise 7

From debugging I saw in the varaibles that remainder_of_sentance becomes empty, because the start_str gets sliced instead of the sentance. 

Fixed remainder_of_sentance on line 10, used sentence instead of start_str when slicing
variable sidebar showed that remiander_of_sentence was empty even though there was still more text in setnace. It was slicing "okay" instead of the sentence. 

Line 13 was the return statement. After the first fix the output remainded to be wrong ( came out as fantastic,kay) I noticed that again it was slicing the start_str, okay -> kay -> ay. Instead of movign through the sentence it was slicing the start_str. I replaced start_str with sentence again to recurse
through the sentence string. 