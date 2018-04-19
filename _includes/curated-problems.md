# Challenges

Solve and review others’ solutions to the list of problems below. We have chosen
these problems carefully as they are similar in difficulty and concepts exercised
to our harder interview questions.

---

# Narcissistic Numbers

### From [Codewars][cw-narcissistic], highly recommend completing there (they have test cases)

A Narcissistic Number is a number which is the sum of its own digits, each raised to the power of the number of digits.

For example, take 153 (3 digits):

```
1^3 + 5^3 + 3^3 = 1 + 125 + 27 = 153
```

and 1634 (4 digits):

```
1^4 + 6^4 + 3^4 + 4^4 = 1 + 1296 + 81 + 256 = 1634
```
### The Challenge:

Your code must return true or false depending upon whether the given number is a Narcissistic number.

Error checking for text strings or other invalid inputs is not required, only valid integers will be passed into the function.

--- 

# Morse Code Decoder

### From [Codewars][cw-morse], highly recommend completing there (they have test cases and a morse code dictionary)


In this challenge you have to write a simple Morse code decoder. While the Morse code is now mostly superceded by voice and digital data communication channels, it still has its use in some applications around the world.

The Morse code encodes every character as a sequence of "dots" and "dashes". For example, the letter A is coded as ·−, letter Q is coded as −−·−, and digit 1 is coded as ·−−−. The Morse code is case-insensitive, traditionally capital letters are used. When the message is written in Morse code, a single space is used to separate the character codes and 3 spaces are used to separate words. For example, the message HEY JUDE in Morse code is ···· · −·−−   ·−−− ··− −·· ·.

NOTE: Extra spaces before or after the code have no meaning and should be ignored.

In addition to letters, digits and some punctuation, there are some special service codes, the most notorious of those is the international distress signal SOS (that was first issued by Titanic), that is coded as ···−−−···. These special codes are treated as single special characters, and usually are transmitted as separate words.

Your task is to implement a function that would take the morse code as input and return a decoded human-readable string.

For example:

```ruby
decodeMorse('.... . -.--   .--- ..- -.. .')
```

should return `"HEY JUDE"`

The Morse code table is preloaded for you as a dictionary (*note*: only on codewars), feel free to use it. It can be accessed in Ruby like `MORSE_CODE['.--']`.

All the test strings would contain valid Morse code.

---

# Count the Smiley Faces


### From [Codewars][cw-smiley], highly recommend completing there (they have test cases)

Given an array (arr) as an argument complete the function countSmileys that should return the total number of smiling faces.

Rules for a smiling face:
- Each smiley face must contain a valid pair of eyes. Eyes can be marked as : or ;
- A smiley face can have a nose but it does not have to. Valid characters for a nose are - or ~
- Every smiling face must have a smiling mouth that should be marked with either ) or D.
- No additional characters are allowed except for those mentioned.

Valid smiley face examples:
```
:) :D ;-D :~)
```

Invalid smiley faces:
```
;( :> :} :] 
```

Example cases:

```ruby
countSmileys([':)', ';(', ';}', ':-D']);       # should return 2;
countSmileys([';D', ':-(', ':-)', ';~)']);     # should return 3;
countSmileys([';]', ':[', ';*', ':$', ';-D']); # should return 1;
```

Note: In case of an empty array return 0. You will not be tested with invalid input (input will always be an array). Order of the face (eyes, nose, mouth) elements will always be the same

---

# Longest Collatz Sequence 

### Adapted from [Project Euler Problem 14][pe-14]

The collatz conjecture concerns itself with a sequence that is generated using a simple set of rules. For all positive integers, the conjecture states that if you follow:

```
if n is even → n/2 (n is even)
if n is odd → 3n + 1 (n is odd)
```

eventually, you will reach the number one.

Using the rule above and starting with 13, we generate the following sequence:

```
13 → 40 → 20 → 10 → 5 → 16 → 8 → 4 → 2 → 1
```

It can be seen that this sequence (starting at 13 and finishing at 1) contains 10 terms. Although it has not been proved yet (Collatz Problem), it is thought that all starting numbers finish at 1.

Which starting number, under one million, produces the longest chain?




---
# nth Prime Number

### Adapted from [Project Euler Problem 7][pe-7]

By listing the first six prime numbers: 2, 3, 5, 7, 11, and 13, we can see that the 6th prime is 13.

What is the nth prime number?

```ruby
  nth_prime(6) => 13 
  nth_prime(10) => 29 
  nth_prime(1000) => 7919
  
  # Last challenge: find the 10001th prime. Note that it make take a while to compute.
```

---

# Amicable Numbers

## Adapted from [Project Euler Problem 21][pe-21]
Let sum_of_proper_divisors(n) be defined as the sum of proper divisors of n (numbers less than n which divide evenly into n).

If we run a number, num1, through the function, we will get num2. What if we run num2 through the function?

If sum_of_proper_divisors(num1) == num2 AND sum_of_proper_divisors(num2) == num1, where num1 != num2, then num1 and num2 are called *amicable numbers*.


For example, the proper divisors of 220 are 1, 2, 4, 5, 10, 11, 20, 22, 44, 55 and 110; therefore sum_of_proper_divisors(220) = 284. The proper divisors of 284 are 1, 2, 4, 71 and 142; so sum_of_properdivisors(284) = 220.

Evaluate the sum of all the amicable numbers under 10000.

--- 

# Largest Prime Factor

### Adapted from [Project Euler Problem 3][pe-3]

The prime factors of 13195 are 5, 7, 13 and 29. Thus, the largest prime factor of 13195 is 29.

What is the largest prime factor of the number 600851475143 ?

--- 

[cw-smiley]: https://www.codewars.com/kata/583203e6eb35d7980400002a
[cw-narcissistic]: https://www.codewars.com/kata/5287e858c6b5a9678200083c/
[cw-morse]: https://www.codewars.com/kata/54b724efac3d5402db00065e
[pe-3]: https://projecteuler.net/problem=3
[pe-7]: https://projecteuler.net/problem=7
[pe-14]: https://projecteuler.net/problem=14
[pe-21]: https://projecteuler.net/problem=21

# Even More Problems!

# Count the palindromes 

Determine how many palindromes are in a string. Order of the
string must be preserved. A palindrome is a string that is 
the same characters reading it forwards as reading it backwards.

Anagram must be of length 3 or more and preserve the given order.

RECOMMENDED: using a helper method to help validate whether a
string is a palindrome or not. is_palindrome?

```ruby
# EX: is_palindrome?("banana") == 2
# there are 2 "ana" anagrams in this example

palindrome_counter("") == 0
palindrome_counter(" ") == 0
palindrome_counter("banana") == 2
palindrome_counter("mississippi") == 6
```

--- 

# Remainder (without modulo)

Determine what the remainder of a non-negative number (n) given 
a divisor the same way modulo is used.

```ruby
def find_remainder(n, divisor)

end

find_remainder(10, 5) == 0
find_remainder(9, 2) == 1
find_remainder(27, 5) == 2
```

---
# Average Movie Ratings

You have a hash of keys that are users and values that are hashes of their movie ratings (also in the form of a hash). The user's movie ratings are also in a hash of key value pairs of movie names and ratings from 1 to 10. Create a hash containing the average ratings for each movies generated from the ratings made by all the users in the input.

Example: 

```ruby
user_ratings = {
   "Ryan" => {"Avengers" => 8, "Little Mermaid" => 8, "Inception" => 9},
   "Clay" => {"Avengers" => 9, "Inception" => 10, "Independence Day" => 7},
   "Christine" => {"Avengers" => 9, "Little Mermaid" => 8, "Inception" => 7},
   "Jon" => {"Avengers" => 5, "Little Mermaid" => 2, "Inception" => 8},
   "David" => {"Avengers" => 3, "Inception" => 8, "Independence Day" => 6}
}

avg_movie_ratings(user_ratings) == {"Avengers"=>6.8, "Little Mermaid"=>6.0, "Inception"=>8.4, "Independence Day"=>6.5}
```