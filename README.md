# Regex_explained

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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
A regex is considered a literal, so the pattern must be wrapped in slash characters (/). If we examine the “Matching a Username” regex, you'll see that this is true:

/^[a-z0-9_-]{3,16}$/


### Anchors
The ^ anchor signifies a string that begins with the characters that follow it. This could be in one of two formats:

 - An exact string match, such as ^The, where the strings "The" or "The person" match, but "the" and "the person" do not. This is because a regex is case-sensitive.

- A range of possible matches, displayed using bracket expressions.

### Quantifiers
Quantifiers set the limits of the string that your regex matches (or an individual section of the string). They frequently include the minimum and maximum number of characters that your regex is looking for.

Quantifiers are inherently greedy, meaning they match as many occurrences of particular patterns as possible. They include the following:

- *—Matches the pattern zero or more times

- +—Matches the pattern one or more times

- ?—Matches the pattern zero or one time

- {}—Curly brackets can provide three different ways to set limits for a match:

- { n }—Matches the pattern exactly n number of times

- { n, }—Matches the pattern at least n number of times

- { n, x }—Matches the pattern from a minimum of n number of times to a maximum of x number of times

### OR Operator
Using the OR operator (|), the expression [abc] could be written as (a|b|c). Using our example in the grouping constructs section, we can take the original expression:

- (abc):(xyz)
And then use the OR operator to convert it to the following:

- (a|b|c):(x|y|z)
Now, both of the strings "abc:xyz" and "acb:xyz" would match, as well as "a:z", but "xyz:abc" would not.

### Character Classes
A character class in a regex defines a set of characters, any one of which can occur in an input string to fulfill a match. We've actually already discussed some character classes. The bracket expressions outlined previously, including positive and negative character groups, are considered character classes.

Here are some of the other common character classes:

- .—Matches any character except the newline character (\n)

- \d—Matches any Arabic numeral digit. This class is equivalent to the bracket expression [0-9].

- \w—Matches any alphanumeric character from the basic Latin alphabet, including the underscore (_). This class is equivalent to the bracket expression [A-Za-z0-9_].

- \s—Matches a single whitespace character, including tabs and line breaks

### Flags
Flags are placed at the end of a regex, after the second slash, and they define additional functionality or limits for the regex. There are six optional flags that can be used, either separately or together and in any order, but these are the three you're most likely to encounter:

-g—Global search: the regex should be tested against all possible matches in a string.

-i—Case-insensitive search: case should be ignored while attempting a match in a string

-m—Multi-line search: a multi-line input string should be treated as multiple lines

### Grouping and Capturing
### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author
A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
