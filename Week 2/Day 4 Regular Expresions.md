# Regular Expressions in Python

Regular expressions, often referred to as regex or regexp, are a powerful tool for searching and manipulating text patterns in Python. They allow you to specify a pattern that can match various strings. Regular expressions are used for tasks like searching, extracting, and validating data. Here's an overview of regular expressions in Python:

## Importing the `re` Module

In Python, regular expressions are supported through the `re` module. You need to import this module to work with regular expressions.

```python

import re

```

## Basic Patterns

### 1.  `re.search(pattern, string)`

The search function searches for the first occurrence of a pattern in a string and returns a match object if found.

```python

import re

text = "The quick brown fox jumps over the lazy dog."
pattern = "fox"
match = re.search(pattern, text)

```

### 2. `re.match(pattern, string)`

The match function attempts to match the pattern at the beginning of the string and returns a match object if successful.

```python

import re

text = "The quick brown fox jumps over the lazy dog."
pattern = "The"
match = re.match(pattern, text)

match = re.search(pattern, text)

```

### Metacharacters

Regular expressions use metacharacters to specify patterns. Some common metacharacters include:

- . : Matches any character except a newline.
- * : Matches 0 or more occurrences of the preceding character.
- + : Matches 1 or more occurrences of the preceding character.
- ? : Matches 0 or 1 occurrence of the preceding character.
- ^ : Matches the beginning of the string.
- $ : Matches the end of the string.
- [] : Matches any character within the square brackets.
- | : Alternation, matches either the pattern on the left or the pattern on the right.

### Character Classes

You can use character classes to match specific types of characters, like digits, letters, or whitespace:

- \d: Matches any digit (0-9).
- \D: Matches any non-digit character.
- \w: Matches any word character (alphanumeric and underscore).
- \W: Matches any non-word character.
- \s: Matches any whitespace character.
- \S: Matches any non-whitespace character.

### Quantifiers

Quantifiers control the number of occurrences a character or group of characters can have:

- {n}: Matches exactly n occurrences.
- {n,}: Matches at least n occurrences.
- {n, m}: Matches at least n and at most m occurrences.

### Groups and Capturing

You can use parentheses to create groups and capture specific parts of the matched string.

```python

import re

text = "John Smith's phone number is 555-1234."
pattern = r"(John Smith's phone number is (\d{3}-\d{4}))"
match = re.search(pattern, text)

```

### Substitution

You can use regular expressions for text replacement using the sub function:

```python

import re

text = "Hello, my name is John. Hello, my name is Alice."
pattern = "Hello"
replacement = "Hi"
new_text = re.sub(pattern, replacement, text)


```

## Regular Expression Flags in Python

Regular expression flags, also known as modifier flags, are used in Python to modify the behavior of regular expressions when searching or matching text patterns. Flags can control case sensitivity, multiline matching, and more. Here's an overview of regular expression flags in Python:

### Importing the `re` Module

Regular expression flags are applied when using the `re` module in Python. To use flags, you need to import the `re` module:

```python
import re

```

### Common Flags

#### 1. `re.IGNORECASE` or `re.I`

The re.IGNORECASE flag is used to perform case-insensitive matching. It allows the regular expression to match characters regardless of their case.

```python
import re

text = "The quick brown Fox jumps over the lazy Dog."
pattern = "fox"
match = re.search(pattern, text, re.IGNORECASE)

```

#### 2. `re.MULTILINE` or `re.M`

The re.MULTILINE flag is used for multiline matching. It allows the ^ and $ metacharacters to match the beginning and end of each line within the text, not just the entire string.

```python

import re

text = "Line 1\nLine 2\nLine 3"
pattern = r"^Line"
matches = re.findall(pattern, text, re.MULTILINE)

```

Regular expressions are a powerful tool for text manipulation and pattern matching in Python. They provide a flexible and expressive way to work with textual data.
