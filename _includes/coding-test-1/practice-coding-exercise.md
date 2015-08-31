## Instructions

This is practice for the coding exercise. It contains
problems of similar difficulty to the actual coding exercise,
but will not be graded. Feel free to take as much time as you
want, but know that the actual coding exercise is timed; to be
adequately prepared, you should be able to complete this within
45 minutes.

Use either your own Ruby setup, or [repl.it](http://repl.it).

The exercise is described with Ruby or Python in mind. However,
you may answer it in any programming language you are most
familiar with. However, please do not write pseudocode.

## lucky_sevens?

Write a function `lucky_sevens?(numbers)`, which takes in an array of
integers and returns true if any three consecutive elements sum to 7.

    lucky_sevens?([2,1,5,1,0]) == true # => 1 + 5 + 1 == 7
    lucky_sevens?([0,-2,1,8]) == true # => -2 + 1 + 8 == 7
    lucky_sevens?([7,7,7,7]) == false
    lucky_sevens?([3,4,3,4]) == false

Make sure your code currectly checks for edge cases (i.e. the first
and last elements of the array).

## oddball_sum

Write a function `oddball_sum(numbers)`, which takes in an array of integers
and returns the sum of all the odd elements.

    oddball_sum([1,2,3,4,5]) == 9 # => 1 + 3 + 5 == 9
    oddball_sum([0,6,4,4]) == 0
    oddball_sum([1,2,1]) == 2

## disemvowel

Write a function `disemvowel(string)`, which takes in a string, and returns that
string will all the vowels removed. Treat "y" as a consonant.

    disemvowel("foobar") == "fbr"
    disemvowel("ruby") == "rby"
    disemvowel("aeiou") == ""

## You're done!

Congrats on finishing the practice coding exercise! When you're ready, feel free
to start the real thing.
