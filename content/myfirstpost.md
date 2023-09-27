---
author: "Peace Sandy"
title: "Regular Expressions in JavaScript"
date: "2022-08-16"
---
![Alt text](javascriptdocumentation.png)

You may have encountered an error while filling out a form, which could be due to an incorrect email address or an invalid password. This error-checking mechanism uses a regular expression, or RegEx in JavaScript, to validate the input. With the help of a regular expression, we can examine a series of characters to determine whether they meet specific criteria. RegEx is short for regular expressions. Regular expressions can be found in many programming languages used today and are used to perform various functions. In this article, we are going to be looking at regular expressions in JavaScript.

## RegEx (Regular Expressions)
Regular expressions are used to create patterns matching different parts of a string. Using a regular expression, you can define practices like; a letter preceded by a hyphen, a symbol followed by a number, or a bunch of different characters in a defined order. Regular expressions are supported in many other programming languages, and they have similar concepts. What this means is that a regular expression in one language will most likely achieve the same result in another language. However, there can be slight differences, which depend on the programming language or the Regex engine running the expression. Also, there can be multiple regular expressions for different patterns. Regular expressions can be used to define patterns.

## Why Regular Expressions?
Regular expressions have become very useful in programming, they can be used to achieve the following:

1. Regular expressions can be used to find the parts of a sting that match a pattern. It can be used to search for a match in a particular piece of content.

2. They are also used to validate that a string follows a pattern. e.g., to verify that an email string is valid.

3. Regular expressions can also be used to verify if a password meets certain criteria.

## How Regular Expressions Work
Programming languages come with Regex engines that execute regular expressions defined by the users. These engines are responsible for finding and returning the parts of a string that match the regular expression created by the user. The engine searches through the string from left to right when applying the regular expression. This method uses the backtracking regex engine.

## RegEx Syntax
Regular expressions are objects that can be created using the RegExp constructor or by enclosing a pattern in forward slash (/) characters and writing it as a literal value. Both literal notations and the RegEx constructor can be used to create regular expressions.

`const regExpStr = 'Hi Everyone! hi everyone'`
<br>
// Syntax: /pattern/flags
`const regExpLiteral = /Hi/gi`

`console.log(regExpStr.match(regExpLiteral))`
// Output: ['Hi', 'hi']

<br>

The RegEx constructor accepts two arguments
`let RegExp = (pattern, flags)`

## Terms used in RegEx
When using Regular Expressions, you may encounter various terminologies. Today, we will explore the commonly used terminologies in Regular Expressions.

**String:**
<br>
A string is a combination of characters; this can be a letter, a word, or a sentence. When a pattern is applied to a string, you can get the parts of that string (substring) that match the defined pattern. Substring refers to specific parts of the whole string. A string can be made up of different characters.

 **Letters:**
 <br>
 When you come across the letter casing, it can either be uppercase or lowercase.

**Symbols:**
<br>
A symbol is a character or a sign, they are special characters, that have meanings. examples include: $ , ^ , & ,* , @ , ! etc.

**Whitespace:**
<br>
This refers to the horizontal or vertical space between characters. Horizontal space can be obtained by clicking on the single & tab spaces, while vertical is the newline space, which is the space between one line and the other, or line break.

**Character:**
<br>
Characters refer to digits, letters, symbols, or whitespace. All of these are classified as characters.

**Pattern:**
<br>
In simple terms, what you are looking for can match a combination of characters in a string.

**Flags:** 
<br>
Most regular expressions have some default behaviors; these flags are optional characters that can be added at the end of your pattern to change some of those default behaviors.

<br>

## Modifiers
Flags, also known as modifiers, are additional parameters that can be passed to regular expressions to alter their default behavior. These modifiers can be used to specify how you want to match the expression. In literal notation, these modifiers are added to the end of the last forward slash (/) used in the expression.
There are four common flags in Regex, they include;

**g-Global:** 
<br>
By default, a regular expression only matches the first set of characters in a string. However, using the global flag g returns all matches.

**i-case-insensitive:**
<br>
The case-insensitive flag removes all case restrictions in the matches. By default, regular expressions are case-sensitive; to change the pattern, use the flag.

**s-Newline flag:**
<br>
 By default, the dot sign . is a special character that matches any kind of character except a newline. To remove the default, you can add s flag.

**m-multiline match flag:** 
<br>
The symbol /m is used for multiline matches. The symbol ^, which is used at the beginning of a regular expression, matches the beginning of a string. Similarly, the symbol $, which is used at the end of a regular expression, matches the end of a string.

## Regular Expression Methods
There are various methods used in Regular Expression, they include;

**The test() Method:**
<br>
The simplest one is the test() method. The test() method compares the target text with the regex pattern and returns a Boolean telling you if the string contains a match of the pattern in the expression.

`const regExp = /hello/i`;

`console.log(regExp.test('hello'))`; // Output: true

`console.log(regExp.test('peace'))`; // Output: false `

Also, there are string methods that accept regular expressions. 
<br/>
They include;

`.split()`

splits the string into an array using the match(es) as a delimiter

`.match()`

returns an array with the matches

`.matchAll()`

method returns an iterator of results after matching a string

`.search()`

Returns the index of the first match in a string

`.replace()`

replaces a match in the string with a given substring

## Conclusion

In this article, we have explored the workings of regular expressions, including RegEx syntax, terms commonly used in RegEx, flags, and popular methods used in regular expressions. However, it is important to note that regular expressions are a vast topic, and there is much more to learn beyond what we have covered in this article. To further your understanding of regular expressions, I recommend that you refer to additional resources and continue reading up on the topic.

I hope you found this post insightful.

I'd love to connect with you on [Twitter](http://twitter.com/PeaceSandy3) [LinkedIn](https://www.linkedin.com/in/peace-sandy-bb7a691b0) [GitHub](https://github.com/Peacesandy)

I'll see you in my next blog post. Take care!
