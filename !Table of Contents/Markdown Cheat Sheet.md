### Basic Syntax

| Element                                                                         | Markdown Syntax                                     |
| ------------------------------------------------------------------------------- | --------------------------------------------------- |
| [Heading](https://www.markdownguide.org/basic-syntax/#headings)                 | `# H1   ## H2   ### H3`                             |
| [Bold](https://www.markdownguide.org/basic-syntax/#bold)                        | `**bold text**`                                     |
| [Italic](https://www.markdownguide.org/basic-syntax/#italic)                    | `*italicized text*`                                 |
| [Blockquote](https://www.markdownguide.org/basic-syntax/#blockquotes-1)         | `> blockquote`                                      |
| [Ordered List](https://www.markdownguide.org/basic-syntax/#ordered-lists)       | `1. First item   2. Second item   3. Third item   ` |
| [Unordered List](https://www.markdownguide.org/basic-syntax/#unordered-lists)   | `- First item   - Second item   - Third item   `    |
| [Code](https://www.markdownguide.org/basic-syntax/#code)                        | `` `code` ``                                        |
| [Horizontal Rule](https://www.markdownguide.org/basic-syntax/#horizontal-rules) | `---`                                               |
| [Link](https://www.markdownguide.org/basic-syntax/#links)                       | `[title](https://www.example.com)`                  |
| [Image](https://www.markdownguide.org/basic-syntax/#images-1)                   | `![alt text](image.jpg)`                            |
| [Comments](https://www.markdownguide.org/hacks/#comments)                       | ` %% `                                              |
### Extended Syntax
| Element                                                                                                                                                                             | Markdown Syntax                                                                                                    |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| [Table](https://www.markdownguide.org/extended-syntax/#tables)                                                                                                                      | `\| Syntax \| Description \|   \| ----------- \| ----------- \|   \| Header \| Title \|   \| Paragraph \| Text \|` |
| [Fenced Code Block](https://www.markdownguide.org/extended-syntax/#fenced-code-blocks)                                                                                              | ` ```   {     "firstName": "John",     "lastName": "Smith",     "age": 25   }   ``` `                              |
| [Footnote](https://www.markdownguide.org/extended-syntax/#footnotes)                                                                                                                | `Here's a sentence with a footnote. [^1]      [^1]: This is the footnote.`                                         |
| [Heading ID](https://www.markdownguide.org/extended-syntax/#heading-ids)                                                                                                            | `### My Great Heading {#custom-id}`                                                                                |
| [Definition List](https://www.markdownguide.org/extended-syntax/#definition-lists)                                                                                                  | `term   : definition`                                                                                              |
| [Strikethrough](https://www.markdownguide.org/extended-syntax/#strikethrough)                                                                                                       | `~~The world is flat.~~`                                                                                           |
| [Task List](https://www.markdownguide.org/extended-syntax/#task-lists)                                                                                                              | `- [x] Write the press release   - [ ] Update the website   - [ ] Contact the media`                               |
| [Emoji](https://www.markdownguide.org/extended-syntax/#emoji)  <br>(see also [Copying and Pasting Emoji](https://www.markdownguide.org/extended-syntax/#copying-and-pasting-emoji)) | `That is so funny! :joy:`<br>[Emojipedia](https://emojipedia.org/most-popular)                                     |
| [Highlight](https://www.markdownguide.org/extended-syntax/#highlight)                                                                                                               | `I need to highlight these ==very important words==.`                                                              |
| [Subscript](https://www.markdownguide.org/extended-syntax/#subscript)                                                                                                               | `H~2~O`                                                                                                            |
| [Superscript](https://www.markdownguide.org/extended-syntax/#superscript)                                                                                                           | `X^2^`                                                                                                             |
### Callout Boxes
| Base Type  | Aliases                | Default Icon & Color Association       | General Use Case                                             |
| ---------- | ---------------------- | -------------------------------------- | ------------------------------------------------------------ |
| `note`     | `default`              | **Blue** (Info Icon)                   | General information; basic blockquotes.                      |
| `abstract` | `summary`, `tldr`      | **Blue/Purple** (Clipboard/List Icon)  | Summarizing key points or conclusions.                       |
| `info`     | (None)                 | **Blue** (Info Icon)                   | Informational text, technical details.                       |
| `todo`     | (None)                 | **Blue** (Checkmark Icon)              | Tasks, items to be completed, or future work.                |
| `tip`      | `hint`                 | **Green** (Lightbulb/Tip Icon)         | Helpful suggestions, best practices, or guidance.            |
| `success`  | `check`, `done`        | **Green** (Checkmark Icon)             | Successful results, completed actions, or positive outcomes. |
| `question` | `help`, `faq`          | **Yellow/Orange** (Question Mark Icon) | Posing a question, seeking clarification, or FAQs.           |
| `warning`  | `caution`, `attention` | **Orange** (Warning/Alert Icon)        | Warnings, items needing careful consideration.               |
| `failure`  | `fail`, `missing`      | **Red** (X Mark Icon)                  | Failed steps, missing information, or bad outcomes.          |
| `danger`   | `error`                | **Red** (Stop Sign Icon)               | Critical errors, severe risks, or irreversible problems.     |
| `bug`      | (None)                 | **Red** (Bug Icon)                     | Documenting software bugs or mechanical errors.              |
| `example`  | (None)                 | **Purple** (File/Document Icon)        | Demonstrating a concept with a concrete example.             |
| `quote`    | `cite`                 | **Gray** (Quote Icon)                  | Quoting external sources, literature, or dialogue.           |
#### Advanced Features
- **Custom Title:** You can change the title shown next to the icon by simply typing your title after the type identifier: `> [!tip] My DM Ruling`
- **Foldable Callouts:** You can make any callout collapsable by adding a `+` or `-` right after the type identifier:
    - `> [!faq]+ Are we hidden?` (starts **open** by default)
    - `> [!note]- Character Backstory` (starts **closed/collapsed** by default)
- **Custom Callouts (Advanced):** While the types above are built-in, you can define **custom callouts** (with unique icons and colors) by using a **CSS snippet**. You would then use your custom name as the type identifier: `> [!monster]` (requires CSS to be defined by you)