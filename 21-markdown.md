**Markdown** allows you to organize and emphasize what you're trying to communicate on GitHub. It offers a lean approach to content editing, defines a concise, lightweight syntax that strips out the overhead inherent to HTML. 

*** 
### Emphasize text

```markdown
This is *italic* text.
This is also _italic_ text.
```

This is *italic* text.
This is also _italic_ text.

```markdown
This is **bold** text.
This is also __bold__ text.
```

This is **bold** text.
This is also __bold__ text.

Different emphases can also be mixed.

```markdown
_This is **italic and bold** text_
__This is bold and *italic* text__
```

_This is **italic and bold** text_
__This is bold and *italic* text__

To use a literal asterisk, precede it with an escape character.

```markdown
\_This is all \*\*plain\*\* text\_.
```

\_This is all \*\*plain\*\* text\_.

***
### Declare headings

```markdown
###### This is H6 text
```

###### This is H6 text

***
### Link to images and sites

```markdown
![Link an image.](https://static0.srcdn.com/wordpress/wp-content/uploads/2021/02/Rick-Astley-Never-Gonna-Give-You-Up-Remastered-Header.jpg)
```

![Link an image.](https://static0.srcdn.com/wordpress/wp-content/uploads/2021/02/Rick-Astley-Never-Gonna-Give-You-Up-Remastered-Header.jpg)

```markdown
[Link to google.com](google.com)
```

[Link to google.com](google.com)

***
### Make lists

```markdown
1. First
2. Second
3. Third
```

Ordered list:
1. First
2. Second
3. Third

```markdown
- First
  - Nested
- Second
- Third
```

Unordered list:
- First
  - Nested
- Second
- Third

***
### Build tables

```markdown
First|Second
-|-
1|2
3|4
```

| First | Second |
| ----- | ------ |
| 1     | 2      |
| 3     | 4      |

***
### Quote text

```markdown
> This is quoted text.
```

> This is quoted text.

***

### Work with code

```markdown
This is `code`
```

This is `code`

```markdown 
var first = 1; 
var second = 2; 
var sum = first + second; 
```

```
var first = 1; 
var second = 2; 
var sum = first + second;
```

***
### Mention users and teams

```markdown
@githubteacher
```

***
### Track task lists

```markdown
- [x] First task 
- [x] Second task 
- [ ] Third task
```

- [x] First task 
- [x] Second task 
- [ ] Third task

***
### Slash commands

| Command          | Description                                                                                                             |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------- |
| `/code`          | Inserts a Markdown code block.                                                                                          |
| `/details`       | Inserts a collapsible detail area.                                                                                      |
| `/saved-replies` | Inserts a saved reply. If you add `%cursor%` to your saved reply, the slash command places the cursor in that location. |
| `/table`         | Inserts a Markdown table.                                                                                               |
| `/tasklist`      | Inserts a tasklist. This slash command only works in an issue description.                                              |
| `/template`      | Shows all of the templates in the repositor. This slash command work for issue templates and pull request template.     |
