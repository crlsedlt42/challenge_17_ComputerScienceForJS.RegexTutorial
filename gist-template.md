# Regular Expressions and their Objectives

REGULAR EXPRESSIONS (also known as REGEX) is a pattern matching tool used in a variety of technology fields that are used to find a letter, digit, word, or sequence of digits or letters within in a body text. There are many reasons to use REGEX when it comes to Web Development but these two scenarios stood out the most to me as a junior web developer: User Data Validation and Custom Searches.

User Data Validation patterns in REGEX is used on client-side web development to verify the correct information is being given/typed in order to meet a specific criteria. For example, verifying that a password meets a criteria of having a minimum of 8 characters and within those 8 characters there needs to be a uppercase, lowercase, digit and special character in order to create a new user profile for a social media platform. 
Custom Searches are a necessary tool in Web Development, especially if a web developer of any level of skillset is refractoring code that is 1000 lines or longer. When refractoring an application that has thousands of lines of code it is important to be able to find specific instances in the given code to assure that refactored code/application works better than before it was refactored. There are many languages of code that use different methods to implement object oriented programming and different developers might use some of these methods interchangeably. An example of this would be that a working application has been refractored 7 times by three different web developers. A fourth developer comes along (this could be you) and functions, json data types, const variables, classes are written differently i.e. some are written using camel case and some are written using snake case. The task for the fourth web developer is to make two copies of the code, one using only camel case and the other copy to only use snake case for a paying and loyal client. REGEX will work perfectly in this situation because the fourth web developer can use a custom search to find all instances of both camel case and snake case and then replace the code as necessary. 

REGEX can be used in countless situations which makes REGEX an important soft skill to understand to use and implement as junior web developer for creating new applications or improving on existing code. 

Today I will be using the REGEX below to demonstrate how these sereies of characters are used to verify an email address.

Regex to Verify an Email Address: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

First, here are some key elements of REGEX:

## Table of Contents

- [Regex Componets](#regex-components)

## Regex Components

```
 / [inset REGEX here] /  
```
Regex is denoted by two forward slashes and the regular expression is placed between both forward slashes.

LITERAL CHARACTERS
- Literal Characters in REGEX are the letters and numbers that are being searched for in a body of text/code.

METACHARATERS
- Metacharacters are symbols that have a specific purpose in REGEX
Here are some exampls of metacharacters:
```
 . , * , + , ? , | , ()
```
Above the metacharacters are seperated by commas the functionality of these metacharacters will be shown below.

CHARACTER CLASSES
- Charcater classes are used in REGEX to match literal characters from a given metric as shown here: 

```
[a-z], [0-9]
```

QUANTIFIERS
- Quantifiers are used to specifiy and limit the amount of times a character or group should appear from the body of text/code. In the REGEX the 'n' is the minimum number or occurences and 'm' is the maximum limit of characters in a series of characters as shown here: 

```
{n,m}
```

ANCHORS
- Anchors specify the position where in the body of text/code should occor. These anchors are '^' or '$'.

CAPTURE GROUPS
- Capture groups are denoted by '()' and are used to isolate and extract specific characters from the body of text/code. 


FLAGS
- Flags are specific criteria that you give to your REGEX so that the text body can display more specific elements to suit your specific needs. These are flags that are used in REGEX Global (g), Multiline (m), Unicode (u), and Sticky (y).


```
 /. /
```
 Make the rest 

```
 /? /
```
 Make the the rest of possible pattern optional

## Character Escapes

```
 /w / 
```
The will match with any character, typically any letter in the alphabet

```
 /d / 
```

```
 /s / 
```
This

### Anchors

```
 /^ / 
``` 
This ANCHOR will demonstrate the beginning of a line of text/code in a body of text/code.

```
 /$ / 
```
This ANCHOR will demonstrate the end of a line of text/code in a body of text/code.

```
 /A / 
```
This ANCHOR will demonstare the beginning of an entire body of text/code.

```
 /Z / 
```
This ANCHOR will demonstare the end of an entire body of text/code.


### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

[ | ] : Like in JavaScript, " | " denotes and 'or' argument

### Flags

One example of a is Case-Insensitive (i), this flag will match characters whether or not within the body of text is in uppercase or lower case.

```
\ birdhouse \i
```
This REGEX will find all instances of 'birdhouse' even if they're typed like this: Birdhouse, BirdHouse, BIRDHOUSE, BirdhousE

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

## Resources

https://regexr.com/
