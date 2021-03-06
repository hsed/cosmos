# Java programming style guide

Braces
---
All braces should start on the same line as the method they are delimiting. If a control flow statement contains only one line of code, it should not have any delimiting braces, unless using a complex if-statement where at least one block is more than one line long. If using inline braces, there should be a space between the braces and the code in between.

```Java
if (true) {
	// Code
}

while (true)
	// Code

if (true || false) {
	// One line of code
} else {
	/* More than one line of code,
	** so all blocks should be delimited. */
}

int[] arr = new int[] { 1, 2, 3 };
```

Comments
---
Comments should have a space following the double slashes. Any multiline comments should be created with the /\*\*/delimiters.

```Java
// Single line comment, with space after slashes

/* Multi-line comment,
** with spaces after
** the delimiters. */
```

Control flow statements
---
The parentheses for control flow statements should be one space after the statement. There should be a newline between unrelated statements, i.e. between a `while` and `if` but not between an `if` and `else`. There should be no spaces in between a statement and its block of code. This goes for class declarations as well.
```Java
if (true || false) {
	// Code
} else {
	// Else
}

while (true) {

	// Should be no spaces, unlike this

}

class Foo {
	// No space between declaration and code
}
```

Whitespace
---
Tabs should be tab characters, and not spaces.
