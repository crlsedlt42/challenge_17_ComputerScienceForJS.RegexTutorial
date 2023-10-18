# Regular Expressions and their Objectives

REGULAR EXPRESSIONS (also known as REGEX) is a pattern matching tool used in a variety of technology fields that are used to find a letter, digit, word, or sequence of digits or letters within in a body text. There are many reasons to use REGEX when it comes to Web Development but these two scenarios stood out the most to me as a junior web developer: User Data Validation and Custom Searches.

User Data Validation patterns in REGEX is used on client-side web development to verify the correct information is being given/typed in order to meet a specific criteria. For example, verifying that a password meets a criteria of having a minimum of 8 characters and within those 8 characters there needs to be a uppercase, lowercase, digit and special character in order to create a new user profile for a social media platform. 
Custom Searches are a necessary tool in Web Development, especially if a web developer of any level of skillset is refractoring code that is 1000 lines or longer. When refractoring an application that has thousands of lines of code it is important to be able to find specific instances in the given code to assure that refactored code/application works better than before it was refactored. There are many languages of code that use different methods to implement object oriented programming and different developers might use some of these methods interchangeably. An example of this would be that a working application has been refractored 7 times by three different web developers. A fourth developer comes along (this could be you) and functions, json data types, const variables, classes are written differently i.e. some are written using camel case and some are written using snake case. The task for the fourth web developer is to make two copies of the code, one using only camel case and the other copy to only use snake case for a paying and loyal client. REGEX will work perfectly in this situation because the fourth web developer can use a custom search to find all instances of both camel case and snake case and then replace the code as necessary. 

REGEX can be used in countless situations which makes REGEX an important soft skill to understand to use and implement as junior web developer for creating new applications or improving on existing code. 

Today I will be using the REGEX below to demonstrate how these sereies of characters are used to verify an email address.

Regex to Verify an Email Address: 
```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/i
```

First, here are some key elements of REGEX:

## Table of Contents

- [Regex Componets](#regex-components)
- [Anchors](#anchors)
- [Capture Groups](#capture-groups)
- [Character Classes](#character-classes)
- [Literal Characters](#literal-characters)
- [Quantifiers](#quantifiers)
- [Flags](#flags)


### Regex Components

```
 / [inset REGEX here] /  
```
Regex is denoted by two forward slashes and the regular expression is placed between both forward slashes.

ANCHORS
- Anchors specify the position where in the body of text/code should occor. These anchors are '^' or '$'.

CAPTURE GROUPS
- Capture groups are denoted by '()' and are used to isolate and extract specific characters from the body of text/code. 

CHARACTER CLASSES
- Charcater classes are used in REGEX to match literal characters from a given metric as shown here: 

```
[a-z], [0-9]
```
LITERAL CHARACTERS
- Literal Characters in REGEX are the letters, numbers, and symbols that are being searched for in a body of text/code. In this REGEX example 'birdhouse' is the literal character: 

```
\ birdhouse \
```

METACHARACTERS
- Metacharacters are symbols that have a specific purpose in REGEX
Here are some examples of metacharacters:
```
 . , * , + , ? , | , ()
```
Above the metacharacters are seperated by commas the functionality of some these metacharacters will be shown below.

QUANTIFIERS
- Quantifiers are used to specifiy and limit the amount of times a character or group should appear from the body of text/code. In the REGEX the 'n' is the minimum number or occurences and 'm' is the maximum limit of characters in a series of characters as shown here: 

```
{n,m}
```


FLAGS
- Flags are specific criteria that you give to your REGEX so that the text body can display more specific elements to suit your specific needs. These are flags that are used in REGEX Global (g), Multiline (m), Unicode (u), and Sticky (y).

---
### REGEX EXAMPLE
```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/i
```
---

### Anchors

There are two anchors being used in this example: 
```
 /^ / 
``` 
This anchor will demonstrate the beginning of a line of text/code in a body of text/code.

```
 / $/ 
```
This anchor will demonstrate the end of a line of text/code in a body of text/code.

### Capture Groups
There are three capture groups being used in this REGEX example: 
```
Capture Group 1: ([a-z0-9_\.-]+)
```
```
Capture Group 2: ([\da-z\.-]+)
```
```
Capture Group 3: ([a-z\.]{2,6})
```

### Character Classes
There are two character classes being used in this REGEX example: 
```
Character Class 1: a-z
```
As you can see there are three occurances of this class in this REGEX.
```
Character Class 2: 0-9
```
This class occurs only onces in the REGEX.

### Literal Characters
There are four literal characters being matched in the REGEX example:
```
Literal Character 1: @ (i.e. At Symbol)
```
```
Literal Character 2: _ (i.e. Underscord)
```
```
Literal Character 3: - (i.e. Hyphen)
```
```
Literal Character 4: \. (i.e. Period)
```
The period is used as a metacharacter to denote any character when used on its own in REGEX or can be used to match anything after a specific REGEX parameter. This REGEX will find every instance of the literal character 'bird' in REGEX:
```
\ bird. \
```
By adding the period, REGEX will find every instance of 'bird' even if it's within a compound word like 'birdhouse' as listed in the example of literal characters above. 

### Quantifiers
There are two quantifiers being used in this REGEX example
```
Quantifier 1: + (i.e. The plus/addition symbol)
```
The addition symbol matches the previous REGEX and expects more captured groups if needed.
```
Quantifier 2: {2,6}
```
This quantifier is expecting a captured group with a minimum of two characters but no more than six characters will be selected in the REGEX.

### Flags
There is only one flag being used in this REGEX example:
```
Flag: i
```
This flag denotes case insensitive, simply saying that the REGEX will look for any alphabetic characters regardless of them being uppercase or lowercase. 

## Author

Carlos E. De La Torre

Junior Full-Stack Web Developer

[GitHub Account](https://github.com/crlsedlt42)

## Resources

https://regexr.com/

https://regex101.com/

[ChatGPT](https://chat.openai.com/)

[Learn Regular Expressions In 20 Minutes](https://www.youtube.com/watch?v=rhzKDrUiJVk&t=3s)

[How to Write Regular Expressions Without Going Crazy (Beginners Tutorial)](https://www.youtube.com/watch?v=saABx34CsBE&t=575s)