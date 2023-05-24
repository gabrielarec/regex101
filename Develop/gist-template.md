# Title (replace with your title)

Regex101 is a tutorial that explains how a specific regular expression AKA regex, functions by breaking down each part of the expression and describing what it does.

## Summary
I will be describing "Matching a Hex Value" The code snippet is the following: 
 /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

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
The anchors on the code snippet <strong>` ^#?([a-f0-9]{6}|[a-f0-9]{3})$ ` </strong> are: `^` and `$` <br>
The '^' is called The cadet, and the cadet symbol at the beginning of a regular expression denotes the start of a line or string. It is used as an anchor to specify that the pattern that follows should match at the start of the line or string. <br>
The '$' is called... you guessed it! Its called The dollar sign, and the dollar sign at the end of the regular expression denotes the end of a line or a string. It is used as an anchor to specify that the pattern that precedes should match at the end of the line or string. 

### Quantifiers
The quantifiers on the code snippet <strong> `^#?([a-f0-9]{6}|[a-f0-9]{3})$` </strong> are: `{6}` and `{3}` <br>
The `{6}` is applying to the character class `[a-f0-9]` which matches hexadecimal characters and it's specifying that the preceding pattern `[a-f0-9]` must occur exactly six times. <br>
Similarly, the `{3}` is also applying to the character `[a-f0-9]` and it's specifying that the preceding pattern `[a-f0-9]` must occur exactly three times. -It matches three hexadecimal characters in the form `#xxx` when preceded by `#`.

### OR Operator
The OR Operator on the code snippet <strong>` ^#?([a-f0-9]{6}|[a-f0-9]{3})$ `</strong> is: `| ` <br>
The OR Operator is used to specify alternatives within a pattern and allows the regular expression to match either one pattern to another. In this specific expression the OR operator is used to provide two alternatives for the color code pattern. 

### Character Classes
On the code snippet <strong>` ^#?([a-f0-9]{6}|[a-f0-9]{3})$ ` </strong> there are three character classes involved: `[a-f0-9] ` , `[a-f0-9]{6} ` and `[a-f0-9]{3} `<br>
`[a-f0-9] ` This character class matches any single character that is a lowercase letter `a` to `f` or a digit `0` to `9`. It represents the valid characters in a hexadecimal color code. <br>
`[a-f0-9]{6} ` This character class is followed by `{6}` and it specifies that it should match exactly six characters that are within the range of lowercase letters `a` to `f` or digits `0` to `9` and it represents a group of six hexadecimal characters, which corresponds to the format for a full six digit hexadecimal color code. <br>
`[a-f0-9]{3}`  This character class, followed by `{3}` specifies that it should match exactly three characters that are within the range of lowercase letters `a` to `f` or digits `0` to `9` and it represents a group of three hexadecimal characters, which corresponds to the format for a shorthand three digit hexadecimal color code.

### Flags
On the code snippet <strong> ^#?([a-f0-9]{6}|[a-f0-9]{3})$ </strong> there are no flags specified. 

### Grouping and Capturing
Theres one Grouping and Capturing on the code snippet <strong> ` ^#?([a-f0-9]{6}|[a-f0-9]{3})$ `</strong> <br>
The grouping is inside the parentheses `()` and they serve to group the pattern elements together. In the given expression the group contains two alternatives separated by the `|` symbol. Each alternative represents a pattern for matching hexadecimal color codes.<br>
The capturing mechanism allows you to access the matched content within the group for further processing ot extraction. In this case, the captured value would be the matched hexadecimal color code. 

### Bracket Expressions
The bracket expressions on the code snippet <strong>` ^#?([a-f0-9]{6}|[a-f0-9]{3})$` </strong> is: `[a-f0-9] `  <br> and it defines the allowed character within the hexadecimal color pattern.

### Greedy and Lazy Match
On the code snippet <strong> `^#?([a-f0-9]{6}|[a-f0-9]{3})$` </strong>  the quantifiers used for matching `{6}` and `{3}` are considered greedy by default. <br>
Greedy quantifiers match as much as possible while still allowing the overall match to succeed. In the regular expression `/[a-f0-9]{6}/`, the `{6}` quantifier is greedy. It tries to match exactly six hexadecimal characters `([a-f0-9])` consecutively. This means that if there are more than six hexadecimal characters available, the greedy quantifier will match all six characters, even if a shorter match is possible.
<br>
Lazy quantifiers, denoted by `?` following a greedy quantifier, match as little as possible while still allowing the overall match to succeed.
In the regular expression `/[a-f0-9]{3}/` , the `{3}` quantifier is greedy. It tries to match exactly three hexadecimal characters `([a-f0-9])` consecutively and if we modify the regular expression to `/[a-f0-9]{3}?/` , the quantifier becomes lazy. This means that the lazy quantifier will match the shortest possible sequence of three hexadecimal characters that satisfies the overall pattern.

### Boundaries
The Boundaries on the code snippet <strong> `^#?([a-f0-9]{6}|[a-f0-9]{3})$` </strong> are defined by the anchors `^` and `$` as well as the optional `#` character

### Back-references
In this particular case the back-reference us used to ensure that the color code is either six characters long or three characters long, as specified by the capturing group.

### Look-ahead and Look-behind
The regular expression <strong> `^#?([a-f0-9]{6}|[a-f0-9]{3})$` </strong> does not use Look-ahead and Look-behind assertions. 

## Author

GitHub profile https://github.com/gabrielarec 
