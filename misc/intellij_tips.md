# IntelliJ Tips & Tricks

[IntelliJ IDEA](https://www.jetbrains.com/idea/) is a wonderful IDE with lots of functions that make developer's lives easier. Here I collect a bunch of random things that I really enjoy to use - and hopefully they will help you as well! 🎉

## Tips & Tricks

### How to learn new tricks

The best trick is the one that enables you to learn more tricks! Just press `Shift + Shift`, and you can search for files, settings, functions, classes, actions and so much more! Also this will show you the shortcut for all actions, so it's really nice to learn all those nice shortcuts!

If you're just looking for an action, type `Cmd + Shift + A` on Mac or `Ctrl + Shift + A` on Mac/Linux.

For the rest of this document, I'll only mention the Mac shortcuts for brevity.

### Navigation

- Search files, functions, settings, actions, etc. with `Shift + Shift`
- Jump to line in file e.g. by typing `File:42`
- Jump to class with `Cmd + click`
- Go backward/forward with `Cmd + Alt + Left` or right
- Show/hide tool windows, e.g. `Cmd + 1` for project view

### Editing

- Fix problems and get suggestions with `Alt + Enter`
- Reformat code with `Cmd + Alt + L` (add `Shift` to show options and select *Optimize imports*)
- Insert new things with `Cmd + N`
- Extend / Shrink selection with `Alt + Up` or `Alt + Down`
- Cut lines with `Cmd + X`
- Duplicate line: `Cmd + D`
- Show parameters `Cmd + P`
- Show help `F1`
- Find usages
- Move lines with `Alt + Shift + Up` or down
- Close other tabs

### Refactor

- Show *Refactor this* menu with `Ctrl + T`
- Rename with `Shift + F6`
- Extract variable with `Cmd + Alt + V`
- Extract method with `Cmd + Alt + M`
- Inline with `Cmd + Alt + N`

### Misc

- Copy Maven dependencies (XML) to a Gradle file automatically converts them
- show (Kotlin) bytecode
- Analyze data flow to here

### Scratch files

A scratch file allows you to create a new file without the need to specify a file name or location. They are ideal for lots of things:

- write something down fast
- get instant syntax highlighting for something
- instant way to format something

For example, I get some minified JSON from somewhere. Now I just want to show it nicely to be able to read it.

Let's pull some JSON, minify it (GitHub already pretty-printed the JSON for us, but we revert that for this sample) and copy it to the clipboard:

```bash
curl https://api.github.com/users/mreichelt | jq -Mc | pbcopy
```

Now we create a new scratch file with `Cmd + Shift + N` and select *JSON* in the dropdown, paste the JSON. Now we can reformat the JSON and profit! 🎉

### Version Control (Git)

TODO

### Let IntelliJ fix your code for you with `F2` and `Alt + Enter` (this is fun!)

With `F2` you can go to the next problem in your code. If you have errors, this will be the next one. If no errors exist, this will take you to the next warning. Combined with IntelliJ's help to automatically fix certain issues with `Alt + Enter` in many times you can just improve or fix your code using these two shortcuts! It's magic.

### Error driven development

What if you could write your code like you mean it, and then let IntelliJ help you fill it with life? I name it 'error driven development'.

How it works: you write the algorithm you have in your head top-down without defining the methods. Now IntelliJ marks your code as red. Next, using `F2` to jump to the first error and `Alt + Enter` you can implement every step with IntelliJ's help. Whether that is creating a method, adding a parameter to an existing one or more: I found this a big productivity increase, because it lets me focus on the real code without the need for me to write every method signature myself. 💪

### Column editing mode (multiple cursors!)

Some time ago, I didn't even know this feature existed. And often you wouldn't need it. But there comes the moment that you'll love this feature!

Enable Column editing mode with `Cmd + Shift + 8`.

Now you can create multiple cursors under each other e.g. by using `Shift + down` etc., or select exact positions with `Alt + Shift + click`, or select whole multiple words with `Alt + Shift + doubleclick`. Then edit the heck out of it! Oh, and `Alt + Enter` and a lot more things still work! 😊

Don't forget to disable the column editing mode again with `Cmd + Shift + 8`.

## Links

Here is some awesome content with more tips & tricks for IntelliJ, which you can just follow along - and learn a lot! 🌟

- [IntelliJ Wizardry with Heinz Kabutz](https://javaspecialists.teachable.com/p/intellij-wizardry) (free online course)
- [42 IntelliJ IDEA Tips and Tricks](https://www.youtube.com/watch?v=eq3KiAH4IBI) (Video, 2015)
