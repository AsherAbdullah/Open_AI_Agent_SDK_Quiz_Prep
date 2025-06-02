# Markdown Syntax Quiz

This quiz tests your understanding of Markdown syntax as outlined in the Markdown Guide (Basic Syntax). It includes conceptual questions and practical code-based questions suitable for graduate-level proficiency. Each question is multiple-choice with four options.

## Question 1: Headings
What is the correct Markdown syntax for creating a level 3 heading?

A. `### Heading Level 3`  
B. `# Heading Level 3`  
C. `--- Heading Level 3`  
D. `*** Heading Level 3`

**Correct Answer**: A  
**Explanation**: In Markdown, headings are created using the `#` symbol. A level 3 heading requires three `#` symbols followed by a space and the heading text (e.g., `### Heading Level 3`).

---

## Question 2: Emphasis (Bold and Italic)
Given the Markdown text `**This is _bold and italic_ text**`, how will it render in HTML?

A. `<strong>This is <em>bold and italic</em> text</strong>`  
B. `<b>This is <i>bold and italic</i> text</b>`  
C. `<strong>This is bold and italic text</strong>`  
D. `<em>This is <strong>bold and italic</strong> text</em>`

**Correct Answer**: A  
**Explanation**: In Markdown, `**text**` renders as `<strong>` (bold), and `_text_` renders as `<em>` (italic). Nested emphasis follows the same rules, so `**This is _bold and italic_ text**` renders as `<strong>This is <em>bold and italic</em> text</strong>`.

---

## Question 3: Lists (Ordered)
Which of the following Markdown snippets will produce a correctly formatted ordered list with items numbered 1, 2, and 3?

A. 
```
1. Item one
2. Item two
3. Item three
```
B. 
```
1. Item one
1. Item two
1. Item three
```
C. 
```
- 1. Item one
- 2. Item two
- 3. Item three
```
D. 
```
1) Item one
2) Item two
3) Item three
```

**Correct Answer**: A  
**Explanation**: In Markdown, ordered lists require numbers followed by a period and a space (e.g., `1. Item`). Option A uses sequential numbers, which is standard. Option B uses repeated `1.`, which some Markdown parsers normalize to 1, 2, 3, but it’s not guaranteed. Option C is invalid (mixes unordered and ordered list syntax), and Option D uses incorrect syntax (`1)` instead of `1.`).

---

## Question 4: Lists (Nested)
What is the correct Markdown syntax to create a nested unordered list under an ordered list item?

A. 
```
1. First item
   - Subitem
2. Second item
```
B. 
```
1. First item
- Subitem
2. Second item
```
C. 
```
1. First item
   * Subitem
2. Second item
```
D. 
```
1. First item
  - Subitem
2. Second item
```

**Correct Answer**: A  
**Explanation**: Nested lists in Markdown require indentation (typically 2 or 4 spaces) under the parent list item. Both `-` and `*` are valid for unordered lists, but the indentation must align correctly. Option A uses `-` with proper indentation. Option C is also technically valid in some parsers, but Option A is preferred for consistency. Option B lacks indentation, and Option D has insufficient indentation.

---

## Question 5: Code (Inline)
Which of the following correctly formats the text `print("Hello")` as inline code in Markdown?

A. `'print("Hello")'`  
B. `` `print("Hello")` ``  
C. `**print("Hello")**`  
D. `_print("Hello")_`

**Correct Answer**: B  
**Explanation**: Inline code in Markdown is created by wrapping text in single backticks (`` ` ``). Option B correctly formats `print("Hello")` as inline code. Option A uses single quotes, which don’t produce code formatting. Options C and D apply bold and italic formatting, respectively.

---

## Question 6: Code Blocks
What is the correct Markdown syntax for a fenced code block with Python syntax highlighting?

A. 
```
```python
def hello():
    print("Hello, World!")
```
B. 
```
~~~python
def hello():
    print("Hello, World!")
~~~
```
C. 
```
    ```python
    def hello():
        print("Hello, World!")
    ```
```
D. 
```
```py
def hello():
    print("Hello, World!")
```
```

**Correct Answer**: A  
**Explanation**: Fenced code blocks in Markdown use triple backticks (``````) or tildes (`~~~`). The language identifier (e.g., `python`) follows the opening fence for syntax highlighting. Option A is correct. Option B is also valid (tildes work in some parsers), but Option A is more standard. Option C has incorrect indentation, and Option D uses an unofficial shorthand (`py`).

---

## Question 7: Blockquotes
How will the following Markdown render in HTML?

```
> This is a blockquote.
> It spans multiple lines.
```

A. 
```html
<blockquote>
  <p>This is a blockquote.</p>
  <p>It spans multiple lines.</p>
</blockquote>
```
B. 
```html
<blockquote>
  <p>This is a blockquote. It spans multiple lines.</p>
</blockquote>
```
C. 
```html
<p>
  > This is a blockquote.<br>
  > It spans multiple lines.
</p>
```
D. 
```html
<div class="blockquote">
  <p>This is a blockquote.</p>
  <p>It spans multiple lines.</p>
</div>
```

**Correct Answer**: B  
**Explanation**: In Markdown, blockquotes are created with `>` at the start of each line, and multiple lines within the same blockquote are combined into a single `<p>` tag within a `<blockquote>` tag, unless separated by a blank line. Option B correctly reflects this rendering.

---

## Question 8: Links
Which Markdown link syntax is correct for an inline link to `https://example.com` with the text "Visit Example"?

A. `[Visit Example](https://example.com)`  
B. `Visit Example<https://example.com>`  
C. `[Visit Example]<https://example.com>`  
D. `(Visit Example)[https://example.com]`

**Correct Answer**: A  
**Explanation**: Inline links in Markdown use the format `[link text](URL)`. Option A correctly formats the link. Option B is reference-style link syntax without a reference definition. Option C is invalid, and Option D reverses the syntax.

---

## Question 9: Images
What is the correct Markdown syntax to embed an image with the alt text "Logo" and the source `images/logo.png`?

A. `![Logo](images/logo.png)`  
B. `![images/logo.png](Logo)`  
C. `[Logo](images/logo.png)`  
D. `![Logo][images/logo.png]`

**Correct Answer**: A  
**Explanation**: Markdown images use the syntax `![alt text](image URL)`. Option A correctly specifies the alt text and image source. Option B reverses the syntax, Option C is a link (not an image), and Option D is invalid (reference-style images require a reference definition).

---

## Question 10: Horizontal Rules
Which of the following Markdown snippets creates a horizontal rule?

A. `---`  
B. `***`  
C. `___`  
D. All of the above

**Correct Answer**: D  
**Explanation**: In Markdown, horizontal rules can be created with three or more hyphens (`---`), asterisks (`***`), or underscores (`___`), on a line by themselves. All options are valid.

---

## Question 11: Escaping Characters
What is the correct way to display the literal text `*emphasis*` in Markdown without rendering it as italicized text?

A. `\*emphasis*`  
B. `\\*emphasis*\\`  
C. `` `*emphasis*` ``  
D. `**emphasis**`

**Correct Answer**: A  
**Explanation**: To prevent Markdown from interpreting special characters, you escape them with a backslash (`\`). Option A correctly escapes the asterisks to display `*emphasis*` literally. Option B over-escapes, Option C formats it as code, and Option D renders as bold.

---

## Question 12: Paragraphs and Line Breaks
Which Markdown snippet will produce two separate paragraphs?

A. 
```
This is paragraph one.
This is paragraph two.
```
B. 
```
This is paragraph one.

This is paragraph two.
```
C. 
```
This is paragraph one.  
This is paragraph two.
```
D. 
```
This is paragraph one.\n
This is paragraph two.
```

**Correct Answer**: B  
**Explanation**: In Markdown, paragraphs are separated by a blank line. Option B has a blank line between the two sentences, creating two paragraphs. Option A creates a single paragraph with a soft break. Option C forces a line break within one paragraph. Option D’s `\n` is not interpreted as a newline in Markdown.

---

## Question 13: Code Block Edge Case
What happens when you include a fenced code block inside a blockquote?

```
> ```python
> print("Hello")
> ```
```

A. The code block is rendered as a `<pre><code>` block inside a `<blockquote>`  
B. The code block is ignored, and only the blockquote is rendered  
C. The Markdown parser throws an error  
D. The code block is rendered outside the blockquote

**Correct Answer**: A  
**Explanation**: Markdown allows fenced code blocks to be nested within blockquotes. The `>` symbol applies to the entire code block, rendering it as a `<pre><code>` block inside a `<blockquote>` tag.

---

## Question 14: Link Reference Definitions
Given the following Markdown:

```
[example]: https://example.com
Click [here][example] to visit.
```

How will it render in HTML?

A. 
```html
<p>Click <a href="https://example.com">here</a> to visit.</p>
```
B. 
```html
<p>Click [here][example] to visit.</p>
```
C. 
```html
<p>Click <a href="[example]">here</a> to visit.</p>
```
D. 
```html
<p>Click <a href="https://example.com">example</a> to visit.</p>
```

**Correct Answer**: A  
**Explanation**: Reference-style links in Markdown use `[text][id]` with a corresponding `[id]: URL` definition. The Markdown renders as an HTML link with the specified URL and text. Option A correctly shows the rendered output.

---

## Question 15: Complex Formatting
What is the correct Markdown syntax to create a bolded link with the text "Example" pointing to `https://example.com`?

A. `**[Example](https://example.com)**`  
B. `[**Example**](https://example.com)`  
C. `**[Example](https://example.com)**`  
D. `[Example](https://example.com)**`

**Correct Answer**: A  
**Explanation**: To bold a link, the bold markers (`**`) must enclose the entire link syntax `[text](URL)`. Option A correctly applies bold formatting to the link. Options B, C, and D result in incorrect or partial formatting.

---

## Question 16: Edge Case with Lists
What will the following Markdown render as?

```
1. Item one
   - Subitem
   - Another subitem
2. Item two
```

A. An ordered list with two items, the first containing a nested unordered list  
B. An ordered list with one item, followed by an unordered list  
C. Two ordered lists, one nested under the other  
D. A single unordered list with mixed formatting

**Correct Answer**: A  
**Explanation**: The Markdown shows an ordered list (`1.`, `2.`) with a nested unordered list (`-`) under the first item, indented correctly. It renders as an ordered list with a nested unordered list under the first item.

---

## Question 17: Code Block Language Identifier
Which language identifier is most appropriate for a fenced code block containing JavaScript code?

A. `js`  
B. `javascript`  
C. `java`  
D. `script`

**Correct Answer**: B  
**Explanation**: For syntax highlighting, the standard language identifier for JavaScript in Markdown is `javascript`. While `js` (Option A) may work in some parsers, `javascript` is more universally supported. Option C is for Java, and Option D is invalid.

---

## Question 18: Emphasis Precedence
What is the correct rendering of the Markdown `***bold and italic***`?

A. `<strong><em>bold and italic</em></strong>`  
B. `<em><strong>bold and italic</strong></em>`  
C. `<strong>bold and italic</strong>`  
D. `<em>bold and italic</em>`

**Correct Answer**: A  
**Explanation**: In Markdown, `***text***` is interpreted as both bold (`**`) and italic (`*`), with the outer markers applying `<strong>` and the inner applying `<em>`. Thus, `***bold and italic***` renders as `<strong><em>bold and italic</em></strong>`.

---

## Question 19: Practical Code Application
You want to document the following Python code in Markdown with proper formatting and a description. Which is the correct Markdown?

```python
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n - 1)
```

A. 
```
Here is a recursive factorial function:

```python
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n - 1)
```
```
B. 
```
Here is a recursive factorial function:
~~~
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n - 1)
~~~
```
C. 
```
Here is a recursive factorial function:
    def factorial(n):
        if n == 0:
            return 1
        return n * factorial(n - 1)
```
D. 
```
Here is a recursive factorial function:
`def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n - 1)`
```

**Correct Answer**: A  
**Explanation**: Option A uses a fenced code block with the `python` language identifier, which is the standard way to format code with syntax highlighting. Option B uses tildes, which is valid but less common. Option C uses indented code block syntax (less preferred). Option D incorrectly uses inline code formatting.

---

## Question 20: Edge Case with Escaping
What is the correct way to display the literal Markdown syntax `**bold**` in a rendered Markdown document?

A. `\*\*bold\*\*`  
B. `` `**bold**` ``  
C. `\\**bold**\\`  
D. `**bold**`

**Correct Answer**: A  
**Explanation**: To display literal Markdown syntax, special characters like `**` must be escaped with a backslash (`\`). Option A correctly escapes the asterisks. Option B formats it as code, Option C over-escapes, and Option D renders as bold text.
