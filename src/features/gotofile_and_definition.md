# Using Goto File and Goto Definition

<iframe width="640" height="360" src="https://www.youtube.com/embed/U5823J0kYLE" frameborder="0" allowfullscreen></iframe>

Let's say you're workinng a large project containing many files, and you kind-of sort-of know the name of a file that you want to open up. Goto File is our feature to help you quickly and easily jump to any file in your workspace, without the need to search through different directories. Simply hit `Cmd-E` (or `Ctrl-E` on Unix/Windows) and away you go:  
![Goto File Window](./images/gotofile.png)


Goto File offers filtering for any portion of a filename, including directories. Search for the beginning, middle, or end of a file path, or even just an extension, like `.js`, and Goto File with instantly present the results to you. Clicking on a name in the list opens the file right up. Goto File does not support case-insensitive, wildcard (`*`, `?`), or regular expression (`.`, `+`) searching.

Goto Definition takes the same concept and applies it to files. You can easily navigate between classes and members defined in your files. By entering text, you can filter your class' member results. Finally, as you navigate through your file, Cloud9 IDE will jump to the relevant portion of the code:  
![Goto Definition Window](./images/gotodefinition.png)


Note: Currently, Goto Definition only works for Javascript files.