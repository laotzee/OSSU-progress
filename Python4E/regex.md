**What is brittle code?** Code that works when the input data is in a particular format, but is prone to breakage if there is some deviation from the correct format. We call this "brittle code" because it is easily broken
**What is greedy matching?** The notion that  '+' and the asterisk characters in a regular expression expand outwards to match the largest possible string.
**What is grep?** A command available in most Unix systems that searches through text files looking for lines that match regular expressions. The command name stands for 'Generalized regular expression parser'
**What is a regular expression?** A language for expressing more complex search strings. A regular expression may contain special characters that indicate that a search only matches at the beginning or end of a line or many other similar capabilities.
**What is a wild card?** A special character that matches any character. In a regular expression the wild-card character is the period.
**What is the difference between raw strings and regular strings?**
**?**
**?**
**?**
**?**
**?**
**?**
**?**
**?**
**?**
**?**
**?**
**?**
**?**

---
- The task of searching and extracting is common in Python
- re.search('string', stringObject) lets you check if some string is contain in another returning a boolean value

- Raw strings are different from regular strings
- match method = looks for match of the patters at the beginning of the string, returns a match object
- Search method = looks for a match in the entire variable/file, but only once, returns a match object
- *findall method* = looks for the patter in the entire variable/file and return every instance
- *finditer method* = will return a Match object, with span and match attributes for each match of the patter given 
- *Match* objects will have the following attributes: *group, start, end, span*. Where group will return the actual value of the patter, start and end will give the index position of the corresponding value and span will contain the pair slice of the string containing the match
- *Meta Characters* = Characters that have a special meaning
	- The dot character (.) will look for any character except new line.
	- Sets = [Expressions inside square brackets]
		- Looks for single characters instead of whole strings
		- can be used with range [a-z] or [A-Z], [0-9], [a-zA-Z0-9]
	- Quantifiers = * + ?
		- * = 0 or more
		- + = 1 or more		- ? = 0 or 1
		- {x} Specific amount
		- Create date recolector with different formats with sets   