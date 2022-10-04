# Computer Science for JavaScript: Regex Tutorial for Matching Hex Values

Regular expressions match character combinations in strings. In regular expressions, the "^" character means "not". As an example, the letter "a" in a regular expression would "match lowercase a" and when used as "^a" in a rwgular expression, it means "don't match lowercase a".

## Summary

This tutorial is about the elements of a regular expressions used for matching Hex Values. Hexadecimal code is a language where variations of colours across a spectrum are given alphanumeric names to every possible colour type across the spectrum, which ensures absolute accrracy and consistancy when applying colours from a spectrum that allows millions of different individual colours. A hexadecimal color value is a six-digit alphanumeric value with a "#" character at the beginning; it defines the specific colour that is applied to an application. /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)
- [Greedy and Lazy Match](#Greedy-and-Lazy-Match)

## Regex Components

### Anchors

- /^#?([a-f0-9]{6}|[a-f0-9]{3})$/
- Anchors match a position before, after, or between characters rather than matching to the value itself. The term anchor is used because they “anchor” the regex match at a specific position. The "^" character is used to match the position before the first character in the string. Using "^a" to the text "abc" would match "a", but "^b" would not match "abc" because the "b" character cannot be matched right after the start of the string, matched by ^. The "$" character is used in a similar way to match the last character in a string. For example, in same same "abc" string, "c$" would match "c", but "a$" or "b$" would not work when applied to the same example. 

### Quantifiers

- /^#?([a-f0-9]{6}|[a-f0-9]{3})$/
- Quantifiers state the number of characters expected. Quantifiers state the number of instances a character, group, or character class must be in the input for a match to be successful. By default, quantifiers will match as many characters as possible (a term dubbed "greedy"). If the "+", "?" or "{}" characters are used in a regular expression, these characters are considered quantifiers. "?" indicates the expression to match 0 or 1time. As an example Hex Value regular expression where it states {6} (Hex Triplet Format) and {3} (Shorthand Hex Format), this specifies the length of the component before these quantifiers should be 6 for {6} and 3 for {3}.

### Grouping Constructs

### Bracket Expressions

- /^#?([a-f0-9]{6}|[a-f0-9]{3})$/
- Bracket Expressions Match any character specified in square brackets ([]). For example, [dD] [oO] matches do, dO, Do, and DO and gr[ae]y matches both variations of spellings for 'grey'; that is, gray and grey.

### Character Classes

- /^#?([a-f0-9]{6}|[a-f0-9]{3})$/
- Character classes state/define the expected characters in a regular expression. In this example, the character classes are defined in "[]" brackets. The character classes in the example are [a-f0-9] and [a-f0-9] which searches for the same values. In the example. a-f searches for alphabet letters a-f and 0-9 searches for numeric digits 0-9.

### The OR Operator

- /^#?([a-f0-9]{6}|[a-f0-9]{3})$/
- The or operator in regular expressions is defined using "|". The or operator views the components as being seperated by the "|" value in the example that states: ([a-f0-9]{6}``|``[a-f0-9]{3}). This expression states the hex value could be 6 characters [a-f0-9]{6} or 3 characters [a-f0-9]{3}.

### Flags

### Greedy and Lazy Match

- /^#?([a-f0-9]{6}|[a-f0-9]{3})$/
- A "greedy match" will match an element as many times as possible. A lazy match is the opposite and will match an element as few times as possible. In the example, "?" defines the lazy quantifier. The term "lazy" quantifier is given because in this example, the regular expression will match as few occurances as possible. Adding a "?" value would change th lazy quantifier into a "greedy" one which would match all possible/available matches.

## Author

- Created by Huw Richmond

- Github.com/HuwRichmond [GitHub](https://github.com/HuwRichmond)