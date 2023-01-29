# REGEX TUTORIAL - Name Finder

This regex filter was created to find names with differnt formats. For example, many names as we know can start with Dr., Mrs., Mr., etc. This regex filter was created to search for names within documents correctly and efficiently. 

## Summary

The name finder regex correctly and effieciently highlights names of all different formats within a text document. I will be describing how each part of the regex works and what each symbol searches for within the regex. This includes the anchors, quantifiers, grouping constructs, etc. Below you are able to find a sample of the regex: 

namePattern = "(\\w+),\\s(Mr|Ms|Mrs|Dr).?\\s(\\w+)"

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
    This specific regex seems to only have one anchor which is the "" that it starts and ends with. This anchor symbol allows the regex to only search for text since most all names only have text within them. 
### Quantifiers
    Within this regex we can see that there are a couple of quanitifiers. The plus (+) sign is used here (\\w+). This means the regex is matching one or more word characters together. In this case we are capturing the family name or last name first. 
### Grouping Constructs
    As you can see towards the center of the regex contruct there is a grouping
    of name titles. Example: (Mr|Ms|Mrs|Dr). This allows 
### Bracket Expressions
    In this regex there are no bracket expressions. But I know bracket expressions are used to match any one character within the bracket for example, [1234] is matched. On the other hand, [^1234] is allowing the regex to match any one single character BUT 1234 because of the carrot.  
### Character Classes
    In the name finder regex we can see that there is one character class. Though the name titles here are not surrounded in brackets they are still considered name classes since they are searching specifically for the name titles: Mr, Mrs, Dr, etc. 
### The OR Operator
    Once again, we can see that the OR operator is significantly used as amprecends || to search between the different name titles. We can also compare this to if statements we learned in the beginning stages of JavaScript. The double || means OR within an if statement. 
### Flags
    There is one flag within this regex. The lowercase "s" allows the search to include a period or dot. This is because some titles can or cannot have a period. For example, Dr vs Dr. is an example of the s flag at work. 
### Character Escapes
    We can see within this regex there are a few character escapes mostly including the backslash characters. \s means there can either be a period or no period to look for here. Further more \w means there may or may not be a string of literal words here. 
## Author
Jason Chong: 
https://github.com/chongjason914

Jacob Van Dyke: 
https://github.com/jacobvandyke194
