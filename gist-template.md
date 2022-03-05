# RegEX

Welcome to my tutorial describing and helping with getting a better understanding of what RegEx is. By definition RegEx stands for Regular expressions and they are special strings representing a pattern to be matched in a search operation. Now how do we do this by searching for specific patterns with special characters known as unicodes.

## Summary

I will be breaking down the responsibilities of indiviual components of this regular expression: /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/ This expression certifies that a user inputs a valid email address.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors
The two Anchors in regex are "^" and "$".
"^" means that the following code must appear at the beginning of the string.
"$" means that the preceding code must appear at the end of the string. The regular expression contains both of them.
### Quantifiers
the two Quantifiers in this regex includes the "+" and"{ }"
"+" will connect the users email name + email service + .com. 
"{}" for this regex includes {2,6}, which will allow a match range of 2-6 characters for the character set of [a-z\.].
### Character Classes
The Character Class "/d"
"\d" is used to match any digit 0-9 it will only be a single digit like 3 and can not be double lik 15 
### Grouping and Capturing
Grouping and Capturing is done with ( ).
/^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/
Anything within a set of parentheses is taken in a single group, which allows all the information inside to be captured as a single unit.
The first group in this expression is ([a-z0-9_\.-]+) that matches the user email name. The second capturing group is ([\da-z\.-]+) which will match the email service. Then lastly, capture group #3 is ([a-z\.]{2,6}) to capture the .com.
### Bracket Expressions
There are three groups within our code
[a-z0-9_.-], [\da-z.-], and [a-z.]
Bracked expressios for email validation includes the character sets of [a-z0-9_\.-], which is matching any letter a-z and is case senstive. It also matches a character 0-9 and matches the characters "_" , "-" , and "."; [\da-z\.-], which is matching a single digit from 0-9, any character a-z (case senstive), and the characters "." and "-".; [a-z\.] matches any character a-z(case senstive) and the character ".".
### Greedy and Lazy Match
A Greedy Match is created when a regex includes a "+"
The + basically means "as many as possible" of the previous character(s), For example, A+ would match "A", "AA", "AAA", and so on because it will match as many "A"s that may exist in the location.
## Author
My name is Joseph Hudak thanks for taking the time to read this and here is a link to my github https://github.com/Magicalburritos
where you can check out more stuff i am working on.
