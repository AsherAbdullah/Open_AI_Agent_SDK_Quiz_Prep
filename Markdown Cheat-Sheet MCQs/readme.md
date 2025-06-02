# Comprehensive Markdown Quiz (Graduate Level)

This quiz tests your understanding of Markdown syntax and concepts as outlined in the Markdown Cheat Sheet. Each question is designed to challenge your knowledge at a graduate level, covering both theoretical and practical aspects.

---

## Question 1: Headers
What is the correct Markdown syntax to create a level 3 header?

A) `### Header 3`  
B) `#3 Header 3`  
C) `--- Header 3`  
D) `*** Header 3`  

**Correct Answer**: A) `### Header 3`  
**Explanation**: In Markdown, headers are created using the `#` symbol. A level 3 header requires exactly three `#` symbols followed by a space and the header text.

---

## Question 2: Emphasis
Which of the following Markdown snippets will render as **bold** text in all standard Markdown parsers?

A) `*bold*`  
B) `**bold**`  
C) `_bold_`  
D) `__bold__`  

**Correct Answer**: B) `**bold**` and D) `__bold__`  
**Explanation**: Both `**bold**` and `__bold__` render as bold text in standard Markdown parsers. `*bold*` and `_bold_` produce italic text.

---

## Question 3: Code Blocks
Given the following Markdown code block, what will be the rendered output?

```markdown
    ```python
    def hello():
        print("Hello, World!")
    ```
```

A) A syntax-highlighted Python code block  
B) A plain text block without syntax highlighting  
C) A single-line code snippet  
D) An error due to incorrect syntax  

**Correct Answer**: A) A syntax-highlighted Python code block  
**Explanation**: The triple backticks (```) with the language identifier `python` create a fenced code block with syntax highlighting for Python, assuming the Markdown parser supports syntax highlighting (e.g., GitHub Flavored Markdown).

---

## Question 4: Lists
Which Markdown snippet correctly creates a nested unordered list with two levels?

A) 
```markdown
- Item 1
- Item 2
  - Subitem 2.1
  - Subitem 2.2
```

B) 
```markdown
- Item 1
- Item 2
  * Subitem 2.1
  * Subitem 2.2
```

C) 
```markdown
* Item 1
* Item 2
  - Subitem 2.1
  - Subitem 2.2
```

D) All of the above  

**Correct Answer**: D) All of the above  
**Explanation**: In Markdown, both `-` and `*` can be used to create unordered lists, and indentation (typically two spaces) is used to create nested lists. All provided snippets are valid and will render as a nested unordered list.

---

## Question 5: Links
What is the correct Markdown syntax to create a link with the text "Markdown Guide" that points to `https://www.markdownguide.org`?

A) `[Markdown Guide](https://www.markdownguide.org)`  
B) `<Markdown Guide>(https://www.markdownguide.org)`  
C) `{Markdown Guide}[https://www.markdownguide.org]`  
D) `[[Markdown Guide]](https://www.markdownguide.org)`  

**Correct Answer**: A) `[Markdown Guide](https://www.markdownguide.org)`  
**Explanation**: The correct syntax for a link in Markdown is `[link text](URL)`. Option A follows this format exactly.

---

## Question 6: Images
Which Markdown syntax correctly embeds an image with the alt text "Logo" and the source `images/logo.png`?

A) `![Logo](images/logo.png)`  
B) `![images/logo.png](Logo)`  
C) `<img src="images/logo.png" alt="Logo">`  
D) `![Logo][images/logo.png]`  

**Correct Answer**: A) `![Logo](images/logo.png)`  
**Explanation**: Markdown image syntax uses `![alt text](image URL)`. Option A is correct, while option C is HTML, not Markdown, and the others are invalid.

---

## Question 7: Blockquotes
What will the following Markdown render as?

```markdown
> This is a blockquote.
> It spans multiple lines.
```

A) A single-line blockquote  
B) A multi-line blockquote  
C) Two separate blockquotes  
D) Plain text without blockquote formatting  

**Correct Answer**: B) A multi-line blockquote  
**Explanation**: Lines starting with `>` that are consecutive are combined into a single blockquote. The provided Markdown will render as one multi-line blockquote.

---

## Question 8: Horizontal Rules
Which of the following creates a horizontal rule in Markdown?

A) `---`  
B) `***`  
C) `___`  
D) All of the above  

**Correct Answer**: D) All of the above  
**Explanation**: Markdown supports horizontal rules using three or more hyphens (`---`), asterisks (`***`), or underscores (`___`), each on a new line with no other content.

---

## Question 9: Inline Code
What is the output of the following Markdown?

```markdown
Use the `print()` function to output text.
```

A) Use the print() function to output text.  
B) Use the `print()` function to output text.  
C) Use the **print()** function to output text.  
D) Use the *print()* function to output text.  

**Correct Answer**: B) Use the `print()` function to output text.  
**Explanation**: Inline code is created using single backticks (`). The `print()` text will be rendered in a monospaced font, typically as a code snippet, preserving the exact text within the backticks.

---

## Question 10: Tables
Which Markdown snippet correctly creates a table with two columns ("Name" and "Age") and two rows of data?

A) 
```markdown
| Name | Age |
|------|-----|
| Alice | 25  |
| Bob   | 30  |
```

B) 
```markdown
Name | Age
-----|-----
Alice | 25
Bob | 30
```

C) 
```markdown
| Name | Age |
|------|-----|
Alice | 25
Bob | 30
```

D) All of the above  

**Correct Answer**: A) 
```markdown
| Name | Age |
|------|-----|
| Alice | 25  |
| Bob   | 30  |
```  
**Explanation**: Option A is the most correct as it includes proper alignment and spacing. Option B is valid in some parsers (like GitHub Flavored Markdown) but lacks the pipe symbols in the data rows, which may cause issues in stricter parsers. Option C lacks proper spacing, which can lead to rendering issues in some parsers.

---

## Question 11: Task Lists
What is the correct syntax for a Markdown task list with one completed and one incomplete task?

A) 
```markdown
- [x] Completed task
- [ ] Incomplete task
```

B) 
```markdown
- [X] Completed task
- [ ] Incomplete task
```

C) 
```markdown
* [x] Completed task
* [ ] Incomplete task
```

D) All of the above  

**Correct Answer**: D) All of the above  
**Explanation**: Task lists in Markdown (an extension in GitHub Flavored Markdown) use `-` or `*` followed by `[x]` for completed tasks or `[ ]` for incomplete tasks. Both lowercase `x` and uppercase `X` are typically supported.

---

## Question 12: Escaping Characters
What will the following Markdown render as?

```markdown
This is a \*test\* of escaping.
```

A) This is a *test* of escaping.  
B) This is a **test** of escaping.  
C) This is a test of escaping.  
D) This is a *test* of escaping.  

**Correct Answer**: C) This is a test of escaping.  
**Explanation**: The backslashes (`\`) escape the asterisks (`*`), preventing them from being interpreted as emphasis markers. The text renders as plain text with the word "test" not italicized.

---

## Question 13: Code Analysis
Given the following Markdown, identify the error:

```markdown
# My Project

This is a **bold** text and *italic* text.

## Features
- Feature 1
- Feature 2
  - Subfeature 2.1
  - Subfeature 2.2

[Link](http://example.com
```

A) Missing closing parenthesis in the link syntax  
B) Incorrect header syntax  
C) Invalid list indentation  
D) Improper bold and italic syntax  

**Correct Answer**: A) Missing closing parenthesis in the link syntax  
**Explanation**: The link `[Link](http://example.com` is missing a closing parenthesis `)`. The header, list, and emphasis syntax are all correct.

---

## Question 14: Advanced Formatting
Which Markdown snippet correctly creates a definition list (as supported by some Markdown extensions like MultiMarkdown)?

A) 
```markdown
Term
: Definition
```

B) 
```markdown
Term: Definition
```

C) 
```markdown
- Term: Definition
```

D) 
```markdown
> Term: Definition
```

**Correct Answer**: A) 
```markdown
Term
: Definition
```  
**Explanation**: Definition lists, where supported, use the syntax `Term` followed by `: Definition` on the next line, typically indented. The other options are not standard for definition lists.

---

## Question 15: Practical Application
Write a Markdown snippet that includes a level 2 header, an ordered list with two items, and an inline code snippet within the second item. What is the correct syntax?

A) 
```markdown
## My List
1. Item 1
2. Item 2 with `code`
```

B) 
```markdown
## My List
1. Item 1
2. Item 2 with *code*
```

C) 
```markdown
# My List
1. Item 1
2. Item 2 with `code`
```

D) 
```markdown
## My List
- Item 1
- Item 2 with `code`
```

**Correct Answer**: A) 
```markdown
## My List
1. Item 1
2. Item 2 with `code`
```  
**Explanation**: The question specifies an ordered list (using numbers) and a level 2 header (`##`). Option A correctly uses `##` for the header, numbers for the ordered list, and backticks for the inline code.

---

## Question 16: Edge Case
What happens when the following Markdown is rendered?

```markdown
**Bold *italic* text**
```

A) Bold and italic text  
B) Only bold text  
C) Only italic text  
D) Plain text with asterisks  

**Correct Answer**: A) Bold and italic text  
**Explanation**: Nested emphasis is supported in Markdown. The outer `**` applies bold formatting, and the inner `*` applies italic formatting, resulting in text that is both bold and italic.

---

## Question 17: Fenced Code Blocks
Which of the following fenced code block syntaxes will NOT produce a valid code block?

A) 
```markdown
```python
print("Hello")
```
```

B) 
```markdown
~~~
print("Hello")
~~~
```

C) 
```markdown
``` python
print("Hello")
```
```

D) 
ევ

```markdown
```
print("Hello")
```
```

**Correct Answer**: D) 
```markdown
```
print("Hello")
```
```  
**Explanation**: A fenced code block requires at least three backticks or tildes. Option D uses only two backticks, which is invalid and will not render as a code block.

---

## Question 18: Strikethrough
Which Markdown syntax creates strikethrough text (in GitHub Flavored Markdown)?

A) `~~text~~`  
B) `//text//`  
C) `--text--`  
D) `**text**`  

**Correct Answer**: A) `~~text~~`  
**Explanation**: Strikethrough in GitHub Flavored Markdown uses double tildes (`~~`). The other options produce bold text or are invalid.

---

## Question 19: Complex Formatting
Create a Markdown snippet that includes a table, a blockquote, and a code block, all within a single document. Which of the following is correct?

A) 
```markdown
> Quote
> This is a quote.

| Col1 | Col2 |
|------|------|
| A    | B    |

```python
print("Example")
```
```

B) 
```markdown
> Quote
> This is a quote.

| Col1 | Col2 |
|------|------|
A | B

```python
print("Example")
```
```

C) 
```markdown
> Quote
> This is a quote.

Col1 | Col2
-----|-----
A | B

```python
print("Example")
```
```

D) 
```markdown
> Quote
This is a quote.

| Col1 | Col2 |
|------|------|
| A    | B    |

```
print("Example")
```
```

**Correct Answer**: A) 
```markdown
> Quote
> This is a quote.

| Col1 | Col2 |
|------|------|
| A    | B    |

```python
print("Example")
```
```  
**Explanation**: Option A correctly formats a blockquote (with `>` on each line), a table (with proper pipe symbols and dashes), and a fenced code block. Option B lacks pipe symbols in the table data rows, option C lacks proper table header formatting, and option D has an incorrect blockquote format and an invalid code block.

---

## Question 20: Rendering Behavior
What is the expected rendering behavior of the following Markdown in a standard parser?

```markdown
Paragraph 1

Paragraph 2
```

A) Two separate paragraphs  
B) A single paragraph  
C) A bulleted list  
D) A code block  

**Correct Answer**: A) Two separate paragraphs  
**Explanation**: A blank line in Markdown separates paragraphs. The provided Markdown will render as two distinct paragraphs.

---
