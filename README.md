# grader
Compare results of two functions

This function tests two other functions by calling them repeatedly with various input arguments and comparing the results. The inputs to the grader function are two function handles followed by a variable number of additional input arguments. The grader function calls the two other functions with each of the supplied input arguments one by one. If the results match for each input argument, the grader function returns logical true. Otherwise, it returns false. Here are a few sample runs using built-in functions:

grader(@sin,@max,0)

ans =  logical 1


grader(@sin,@max,0,1)

ans =  logical 0


grader(@cos,@cos,-pi,0,pi,[0:0.1:1])

ans =  logical 1
