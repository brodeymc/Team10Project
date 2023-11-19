# Coding Style Guide
This document is the coding style guide for the source code of Computer World. All developers are expected to follow this style guide at **all times**.
## Commenting
Comments should be made frequently enough for current and future developers to understand, but not too frequently as to make reading the program difficult. Assume that readers have experience with Java and understand basic statements.  For example, refrain from comments such as: 

    i = i+1; //add one to i

In the situation where developers are unsure if a comment is necessary, the comment should be added. It is preferable to have unnecessary comments than to be missing potentially important information. **What may seem like common sense to current developers may not be to future developers.**
## Naming Conventions
Adhere to Java's naming conventions, specifically CamelCase (words smashed together and the first letter of each word capitalized).

    thisIsAnExample
The only exemption is constants, which should be written in all-caps with words separated by underscores.

    THIS_IS_AN_EXAMPLE
Names should be descriptive enough to be understood within the context of a method, but not overly descriptive. 
## Formatting
Formatting is important to keep the program readable. While developers have individual preferences for formatting, it is important to maintain consistency within the program.
### Braces
Braces should be placed on individual lines, not on the end of a line.

Example: 

    if (x<y)
    {
		x= y;
		y= 0;
	}
Braces should always be used with `if, else, do` and `while` statements. This remains true when the body is empty.
### Whitespace
Include whitespace in the program to increase readability. Highly condensed code can be difficult to read.

