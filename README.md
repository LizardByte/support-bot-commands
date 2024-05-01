# support-bot-commands

This is a central repository of all the commands that the [support-bot](https://github.com/LizardByte/support-bot)
can execute. The purpose of separating the commands from the bot is to allow for easier updating and
maintenance of the commands.

The commands should be single markdown files and must comply with the following:

| Element                         | Discord                | Reddit                 | Accepted           |
|---------------------------------|------------------------|------------------------|--------------------|
| Headings[^1]                    | :heavy_check_mark:     | :heavy_check_mark:     | :white_check_mark: |
| Paragraphs[^2]                  | :warning:[^3]          | :heavy_check_mark:     | :white_check_mark: |
| Line Breaks                     | :x:                    | :heavy_check_mark:     | :x:                |
| Bold                            | :warning:[^4]          | :heavy_check_mark:     | :white_check_mark: |
| Italic                          | :heavy_check_mark:     | :heavy_check_mark:     | :white_check_mark: |
| Blockquotes                     | :heavy_check_mark:[^5] | :heavy_check_mark:     | :white_check_mark: |
| Ordered Lists                   | :heavy_check_mark:     | :heavy_check_mark:[^6] | :white_check_mark: |
| Unordered Lists                 | :heavy_check_mark:     | :warning:[^7]          | :white_check_mark: |
| Code                            | :heavy_check_mark:     | :heavy_check_mark:     | :white_check_mark: |
| Horizontal Rules                | :x:                    | :heavy_check_mark:     | :x:                |
| Links                           | :heavy_check_mark:     | :heavy_check_mark:     | :white_check_mark: |
| Images                          | :x:                    | :x:                    | :x:                |
| Tables                          | :x:                    | :heavy_check_mark:     | :x:                |
| Fenced Code Blocks              | :heavy_check_mark:     | :heavy_check_mark:     | :white_check_mark: |
| Syntax Highlighting             | :heavy_check_mark:     | :x:[^8]                | :white_check_mark: |
| Footnotes                       | :x:                    | :x:                    | :x:                |
| Heading IDs                     | :x:                    | :warning:[^9]          | :x:                |
| Definition Lists                | :x:                    | :x:                    | :x:                |
| Strikethrough                   | :heavy_check_mark:     | :heavy_check_mark:     | :white_check_mark: |
| Task Lists                      | :x:                    | :x:                    | :x:                |
| Emoji                           | :heavy_check_mark:     | :warning:[^10]         | :white_check_mark: |
| Highlight                       | :x:                    | :x:                    | :x:                |
| Subscript                       | :x:                    | :x:                    | :x:                |
| Superscript                     | :x:                    | :heavy_check_mark:     | :x:                |
| Automatic URL Linking           | :heavy_check_mark:     | :heavy_check_mark:     | :white_check_mark: |
| Disabling Automatic URL Linking | :heavy_check_mark:     | :heavy_check_mark:     | :white_check_mark: |
| HTML                            | :x:                    | :x:                    | :x:                |

:information_source: Do not use features that are not supported by all targets. For example, do not use line breaks,
since it is not supported by Discord.

For more information, see the [Discord Markdown Guide](https://www.markdownguide.org/tools/discord/) or the
[Reddit Markdown Guide](https://www.markdownguide.org/tools/reddit/).

[^1]: A heading is required in every file.
[^2]: Do not exceed 120 characters.
[^3]: Discord does not natively support paragraphs, but we post process the markdown to handle it.
[^4]: Use asterisks. Underscores aren't supported.
[^5]: You can use `>>>` to create a multi-line blockquote.
      All text from the `>>>` to the end of the message will be included in the quote.
[^6]: Lists must start with the number 1.
[^7]: Cannot use plus signs (+).
[^8]: Reddit doesn't support syntax highlighting, but it should be okay to use anyway.
[^9]: Automatically generated. There's no way to set custom heading IDs.
[^10]: Emoji shortcodes are not supported. Paste the emoji directly.
