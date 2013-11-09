NemerleMarkdown
===============

A markdown processor written in Nemerle. It runs on the .NET library, so it can be used for any .NET project, C#, Visual Basic or otherwise.


Output
---------

This project can currently output to `docx` word format, which can then be converted to `pdf` format. The project has been designed to work with different outputs, so future outputs will be added. Here's some planned formats that will be supported:

1. `HTML` - this is the normal output for markdown, so this project will support this as well.
2. `LaTeX` - `LaTeX` is a very awesome format that can be styled and controlled very easily and instantly, and is used for typesetting books (mostly textbooks) and scientific papers. It is very complicated to use however, so having this output to `LaTeX` will get all it's typesetting benefits without having to know `LaTeX`. 
3. `PowerPoint` - divide slides based horizontal rules and headers, and build a slideshow from a markdown document. It will also support `LaTeX` slideshows as well, using a package like `beamer`.
4. `SVG` - A picture format that will leave the text perfectly crisp no matter how zoomed in it is. Other formats such as `PNG` can be created from this format if needed. (`PNG` and other picture formats may be supported directly in the future.

Progress
------------

Markdown is simple to learn, but still rather large, and there's no actual standard format. There are many extensions to Markdown, and eventually this project will support most of the common ones (such as tables and automatic hyperlinking), however the core of Markdown must be implemented first. A specification (sort of) for the core [can be found here](http://daringfireball.net/projects/markdown/syntax). The major elements are listed below along with their progress:

1. **Paragraphs** - Complete, not fully tested
2. **Line Breaks** - Complete, not fully tested
3. **Headers** - Complete, not fully tested
4. **Block Quotes** - Not started
5. **Lists** - Not started
6. **Code Blocks** - Not started
7. **Horizontal Rules** - Not started

As well the following inline elements:

1. **Bold** - Complete, not fully tested
2. **Italics** - Complete, not fully tested
3. **Links** - Partially completed (inline complete, reference not started)
4. **Inline Code** - Not started

Contribution Help
--------------

If you'd like to contribute you need to have Nemerle installed. You may have to fix references to `Nemerle.Peg` and `Nemerle.Peg.Macro` (I've had weird issues with it).

You can contribute by extending the parser to support more of the core syntax