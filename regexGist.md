# REGEX TUTORIAL - Name Finder

This regex filter was created to find names with differnt formats. For example, many names as we know can start with Dr., Mrs., Mr., etc. This regex filter was created to search for names within documents correctly and efficiently. Regular Expressions are impotant to developers because it allows them to find string variations in their code. Since many coding projects are hundreds of thousands of lines of code. Having a regex function can allow simplistic and customizable searches.

## Summary

The name finder regex correctly and effieciently highlights names of all different formats within a text document. I will be describing how each part of the regex works and what each symbol searches for within the regex. This includes the anchors, quantifiers, grouping constructs, etc. Regex are important tools developer can utilize to easily be able to search for strings of code. It is further important since you are completely able to customize regex to your needs. Nowadays we as developers are looking to not only create working code but quicker code as well. Below you are able to find a sample of the regex: 

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
   Anchors match a position before, after or between characters. They quite literally anchor the regex matching string to a certain position.  This specific regex seems to only have one anchor which is the "" that it starts and ends with. This anchor symbol allows the regex to only search for text since most all names only have text within them. 
### Quantifiers
    A quantifier within regular expressions are repeats a string token as many times as possible. This specific quantifier is not backtracking but instead continuously looking through every single string for the required character. Another key characteristic of quantifiers include not releasing string matches as the data backtracks. This can be essential as JavaScript is a variable based language. Within this regex we can see that there are a couple of quanitifiers. The plus (+) sign is used here (\\w+). This means the regex is matching one or more word characters together. In this case we are capturing the family name or last name first. 
### Grouping Constructs
    Some key characteristics regarding grouping constructs include, matching a subexpression that is repeated in the input string, applying quantifiers to as subexpression that is repeated and retreaving subexpressions from string matches! As you can see towards the center of the regex contruct there is a grouping
    of name titles. Example: (Mr|Ms|Mrs|Dr).
### Bracket Expressions
    A bracket expression is a matching list expression or a non-matching list expression. It can contain of one or more expressions including, ordinary characters, collating elements, collating symbols, equivalence classes, character classes, and/or range expressions. In this regex there are no bracket expressions. I know bracket expressions are used to match any one character within the bracket for example, [1234] is matched. On the other hand, [^1234] is allowing the regex to match any one single character BUT 1234 because of the carrot.  
### Character Classes
    In a regular expression we can tell it to match certain string variations. For example, "grey" vs "gray". We can see that they are the same work by spelt differerntly. Using character classes we can grab "grey" by itself by using g[re]y character class. This can be important to developers who are trying to find mistakes in their work.  In the name finder regex we can see that there is one character class. Though the name titles here are not surrounded in brackets they are still considered name classes since they are searching specifically for the name titles: Mr, Mrs, Dr, etc. 
### The OR Operator
    To me the OR operator is one of the most significant tools you can use in a regular expression. This is because some developers, users etc may use different variations of titles, names, and other things. Having an OR operator simplifies this mess by allowing the regex to continue its search if something is not consistent. We can once again, we can see that the OR operator is significantly used as amprecends || to search between the different name titles. We can also compare this to if statements we learned in the beginning stages of JavaScript. The double || means OR within an if statement. 
### Flags
    Flags withing a regular expression are vital for finding punctuation, upper vs lowercase and even multiline strings! Though there are only six flags within JavaScript regex they are quite useful. For example, 'i' is a flag used to search for case sensitivity. It allows the regex to search for both "a" and "A". There is one flag within this regex. The lowercase "s" allows the search to include a period or dot. This is because some titles can or cannot have a period. For example, Dr vs Dr. is an example of the s flag at work. 
### Character Escapes
    There can be small issues when searching for strings within code. For example, we can see there are typos and punctuation after some string sets. Adding a character escape to your regex allows devs to grab all neccessary information regarding their needs. For example, ".+" allows the regex to see if there is more punctuation after the punctuation. That specific example would find something like "?!" in a sentence! We can see within this regex there are a few character escapes mostly including the backslash characters. \s means there can either be a period or no period to look for here. Further more \w means there may or may not be a string of literal words here. 
## Author
Jason Chong: 
https://github.com/chongjason914

Jacob Van Dyke: 
https://github.com/jacobvandyke194
