# Title (replace with your title)

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

### Anchors
Anchors are used at the beginning and end of searches to check if a string matches a certain pattern and they do not match any other characters. They are there to affirm a string matches a location. Achors will create parameters.

Use the ^ anchor to match the beginning of the text.
Use the $ anchor to match the end of the text.
### Quantifiers
Quantifiers will measure and set the limit on the number of characters that we are wanting to match our Regex:

+ Searches the pattern one or more times,
? Searches the pattern zero or one time
* Searches the pattern zero or more times
https? for example. The ? will make the preceeding time optional.
### OR Operator
The OR operator's purpose is to match the characters on the left or right of the operator, serving as an or, as in and/or.

Using the | as in m|M would match either m or an M from the string.
If we had used https?:\/\/(www\.)?[\d-a|A it would search for a OR A.
### Character Classes
A character class is the set of characters that could occur in a string.

The \d character class in the above code is looking for any digits
The \D looks for non-digits
\s searches for space symbols, tab and newlines
\S searches for all but \s
Any character with the regex 's' flag, while the included \w character is looking for an alphanumeric character
### Flags
Flags are used at the end of a regex, after a closing slash. They are toeksn that will modify the parametes of a search. Many flags can be set by writiing one after the other with no spaces. Flags mst be written in lowercase. The URL does not contain any flags.

An example of a flag would be if the above expression showed:
https?:\/\/(www\.)?[\d-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)g

Other Flag Expressions:

u: Unicode. Expression assumes individual characters are code points, not code units and will then match 32 bit characters.
y: Sticky. Indicates that it matches only from the index indicated by the lastIndex property of this regular expression in the target string (and does not attempt to match from any later indexes)
i: Ignores casing. Makes expression case-sensitive
g: Global. Makes expression search for all occurences
s: Dot All. Makes the wild characters . match newlines as well
m: Multiline. Makes boudnary characters ^ and $ match beginning and end of every line.
### Grouping and Capturing
Capturing Group is a part of a pattern that can be enclosed in a parentheses () and is a way to treat multiple characters as one unit.

The example expression has many groupings such as:
https?:\/\/ which is looking for the http(s)
(www\.)?[\d-a-zA-Z0-9@:%._\+~#=] which will look for initial domain
[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=] looks for top level domain
and *) file paths.
### Bracket Expressions
Bracket expressions are matching or non-matching list expression and consists of one or more expressions that will be found in square brackets []

It represents a special character class and is a quantified rule providing range construct.
They adapt to a users or applications locale.
### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
