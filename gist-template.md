# Regex tutorial to validate an email address

Regex, or regular expressions, are and sequence of characters which can define and validate a specific pattern. Regular expressions can be a combination of letters, numbers, special characters, and quantifiers. 



## Summary

Today i will be covering and breaking down the compenents of regular expressions that are used to validate an email address.
This is the regex code that we will analyze today: `/^w+[+.w-]*@([w-]+.)*w+[w-]*.([a-z]{2,4}|d+)$/i`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
The anchors that we use to contain this particular Regex are `^` to start and `$` to finish.

### Quantifiers
In our example regex we used  `+` a few times in our expression. This is an example of a greedy quantifier. We also used `{2,4}` towards the end of the expression, this is another greedy quantifier that specifies the input needs to be a minimum of 2 characters but no more than 4 characters.

### OR Operator

### Character Classes
In our regex, the character class `\w` is used. Jacascript classifies this as a use of any word (letters, digits, underscores).

### Flags
In JavaScript, when we are talking about flags, there are only six flags that work with JavaScript and retro regular expressions; those are “I,” which is a flag that searches for casein sensitive. There is a G; this flag looks for anything without the specified request. M is multiline and makes it so that you can use a dot to match. Finally, the character U flag helps to process pairs correctly, and y is the sticky flag it looks for a particular position. https://javascript.info/regexp-introduction

### Grouping and Capturing
There are three groups being captured in out example. The first is: `/^w+[+.w-]*@`. This is the "user name" and it captures everything before the `@`. The second group is: `([w-]+.)*w+[w-]*.`. This is the "domain name" and it captures everything in between the `@` and the `.`. The third and final group: `([a-z]{2,4}|d+)$/i` captures the "extension", or everything that comes after the `.`. (i.e .com or .net)

### Bracket Expressions
We have four different bracket expressions in out example expression! The information inside of the bracket is held in open/close bracketsm like this `[]`. This identifies which information is matched.

### Greedy and Lazy Match
In our example we only have greedy matches,  `+` and `{}`. This means that it will allow the match to expand as long s it needs to. If we were to have used lazy quantifiers, then they would look like `+?` and `{}?`. These would direct the system to make the shortest match it can. 

### Boundaries
Word boundary, exhibited with a (\b) it is equivalent to an anchor. It tells the user that this is a word boundary. It is a way to declare here a word/this is a word boundary. Example “fish” within the parenthesis is a word. If a particular regex declared, with anchors, “this is the first of a regex string,” using a ^ carrot, or the end of a string with the dollar sign, then a space or place is being declared. \b asks the programing language to look for that whole word. for example, if we said, please find the entire word “fish.” There are more complexities involved, but that’s a basic idea. https://www.javascripttutorial.net/regular-expression-word-boundaries/


### Back-references
Back-references What does a back-reference look like? It is typically a \ followed by single-digit. Back-reference is a command, which refers to something that already happened or a previous part of a matched regular expression. You could make a better preference by name or number; basically, what you are doing is you are referencing a named group, and you would have a bag/and a K then the name of that group, for example.


### Look-ahead and Look-behind
Look ahead and look behinds allows how matches get handled when using regular expressions. I looked at the website regex buddy also says regular Dash expression .info, and Specifically, I looked at look-ahead and look-behind zero-length assertions on this website. Look ahead and look behinds, also known as look around assertions, are similar to a start and end of the line or anchors. However, look around can match characters, and then they return a result of either a match or no match.



## Author

My name is Oscar Hurtado my Github link: https://github.com/OscarH1025