# Regex Tutorial

Regular expressions, or regex for short, are powerful tools used in computer science and programming for searching and manipulating text. A regex is essentially a pattern of characters that describes a specific search pattern. By using a combination of regular expression syntax and search algorithms, you can use regex to match specific text patterns, validate user input, extract data from text, and perform a wide range of text processing tasks. While learning regex can be daunting at first, it is a valuable skill to have for anyone working with text data.

## Summary

Regular expressions, or regex, are powerful tools used for searching and manipulating text. They consist of a sequence of characters that form a search pattern, which is used to match and extract specific pieces of information from a larger string or document.

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
There are two main types of anchors in regular expressions: the caret (^) and the dollar sign ($). The caret anchor matches the beginning of a line, while the dollar sign anchor matches the end of a line.
### Quantifiers
* - Matches zero or more occurrences of the preceding character or group. For example, the pattern a* would match "a", "aa", "aaa", and so on.

+ - Matches one or more occurrences of the preceding character or group. For example, the pattern a+ would match "a", "aa", "aaa", but not an empty string.

? - Matches zero or one occurrences of the preceding character or group. For example, the pattern colou?r would match both "color" and "colour".

{n} - Matches exactly n occurrences of the preceding character or group. For example, the pattern a{3} would match "aaa", but not "aa" or "aaaa".

{n,} - Matches at least n occurrences of the preceding character or group. For example, the pattern a{2,} would match "aa", "aaa", "aaaa", and so on.

{n,m} - Matches between n and m occurrences of the preceding character or group. For example, the pattern a{2,4} would match "aa", "aaa", and "aaaa", but not "a" or "aaaaa".
### OR Operator
In regex, the OR operator allows you to search for alternative patterns within a string. It is represented by the | symbol and can be used to match any one of several patterns. For example, the regular expression cat|dog will match either the string "cat" or the string "dog".
### Character Classes
[a-z]: matches any lowercase letter from a to z
[A-Z]: matches any uppercase letter from A to Z
[0-9]: matches any digit from 0 to 9
[aeiou]: matches any vowel character
[^aeiou]: matches any non-vowel character
### Flags
i (ignore case): This flag allows the regular expression to match both uppercase and lowercase letters regardless of the case used.
Example: /hello/i would match "hello", "HELLO", "Hello", etc.

g (global): This flag allows the regular expression to match all occurrences of a pattern rather than just the first one.
Example: /cat/g would match "cat" in "The cat sat on the mat" and "The cat chased the rat".

m (multiline): This flag allows the regular expression to match across multiple lines in a string.
Example: /^hello/m would match "hello" at the beginning of each line in a multiline string.

s (dotall): This flag allows the dot (.) character in a regular expression to match any character, including newline characters.
Example: /.+/s would match any sequence of characters, including newlines.

u (unicode): This flag enables full Unicode support for the regular expression.
Example: /\p{Script=Greek}/u would match any Greek character in a Unicode string.

y (sticky): This flag causes the regular expression to perform a "sticky" search, meaning that it will match only at the current position in the string.
### Grouping and Capturing
In regular expressions (regex), grouping and capturing are used to capture a specific part of a matching pattern. This allows you to extract specific parts of the matched string that you need, while ignoring the rest.
### Bracket Expressions
In regular expressions, a bracket expression is a way to match a single character from a specified set of characters. It's used to define a range or set of characters to match against. The brackets are used to enclose the set of characters to match, and the characters are specified inside the brackets.
### Greedy and Lazy Match
In regular expressions, quantifiers such as *, +, and ? are greedy by default, which means they will match as much as possible of the input text that fits the pattern. However, in some cases, you may want to make a quantifier lazy, which means it will match as little as possible of the input text that fits the pattern.
### Boundaries
Word boundaries: Matches the position between a word character (as defined by \w) and a non-word character (as defined by \W).
Syntax: \b

Beginning and end of the line: Matches the position at the start or end of a line.
Syntax: ^ for the beginning of the line, $ for the end of the line.

Lookaround assertions: Matches a pattern only if it is followed or preceded by another pattern.
Syntax:

Positive lookahead: (?=pattern)
Negative lookahead: (?!pattern)
Positive lookbehind: (?<=pattern)
Negative lookbehind: (?<!pattern)
Here are some examples of how bound
### Back-references
In regular expressions (regex), backreferences are used to refer to previously matched subpatterns within a pattern. Backreferences are indicated by using backslashes followed by a number (e.g. \1, \2, etc.) to reference the corresponding group that was matched.
### Look-ahead and Look-behind
Look-ahead and Look-behind are regex constructs that allow for searching patterns that are followed or preceded by specific patterns without including those specific patterns in the match. They are also called zero-width assertions, as they do not actually match any characters in the input string, but rather assert a certain condition.
## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
