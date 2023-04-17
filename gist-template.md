# Regular Expression Tutorial

In this tutorial you will be learning about regular expressions, also known as regex.

## Summary

This  tutorial will explain the regular expression `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`, which is a used to search for emails.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Character Escapes](#character-escapes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Anchors

^ and $ are both anchors in this regex. ^ signifies that the regex will search for phrases starting with whatever comes after it, while $ signifies that the regex will search for phrases ending with whatever preceded it. These anchors are used to determine what parts of the regex should determine the start or end of what it searches for.

### Quantifiers

+ and {2,6} are both quantifiers in this regex. the + quantifier means that the phrase must match the provided pattern 1 or more times and is used to determine that the part of the email before and after the @ symbol exsist. the {2,6} means that the phrase must match the pattern from 2 to 6 times and is used to determine that the final part of the email after the period is 2-6 characters long.

### Character Classes

a-z, 0-9, amd \d are all character classes in this regex. a-z means that it can contain any lower case letter while 0-9 and \d are both different ways of specifying it can contain any numerical digit. These are used so that the regex can contain any letters and numbers in the sections of the email before and after the @ symbol, and only alphabetic characters after the period towards the end of the email.

### Character Escapes

\ can be used as a character escape which causes a special character to be interpretted as a literal character instead. This regex uses \. so that the periods are interpreted as literral because they would otherwise signify any character type.

### Grouping and Capturing

parrenthesis () are used for seperating the regen into sections which must be found one after another. In our regex this is used to determine the section of the email before the @, the section after the @ but before the period, and the the secion after the period all seperately and in order.

### Bracket Expressions

bracket expressions are used to create a character group where the string the regex searches for can be met with any of the contained characters. The email regex uses [a-z] and [0-9] to allow any lowercase alphabetic or numberic characters to be used in the main sections of the email (the final section only had [a-z] so numbers are not allowed).

## Author

My name is Ryan Massenburg and I am a student at UW coding bootcamp. you can checkout my github at https://github.com/chulleyboy
