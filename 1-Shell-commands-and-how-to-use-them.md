# Shell commands and how to use them

You probably interact with your computer by moving your mouse around the screen to click on things, open files, play games, etc.
This is called using the Graphical User Interface. 

The other way to use your computer is by using the command line, often called the shell. You know, the black screen with only text on it that hackers always use in movies. Shell commands are what you type into the shell to do things.

This is quite useful, and often faster than using a mouse to do things.

As a developer, you will use the shell to do lots of things, including but not limited to:
- Creating, editing, and deleting files and folders
- Navigating your files and folder

In fact, that's probably all you need to know for now, so here's how to do that.

## Open the Command Line
If you're on Mac, click on Finder -> Applications and open Terminal.

An easier way to do this is hit Ctrl-Space, type in Terminal, and hit enter.

## Navigate your folder structure
If you are used to using Finder to view your files on Mac, you know that Finder opens into your home directory. If you want to view pictures, then you have to click on the Pictures folder before you can see your picture files.

The command line works the same way. When you open the command line, it opens up to your home directory.

Don't believe me? Try using `pwd`

## `pwd` - Show the current directory

Type this into your command line and you will what folder the command line thinks is your home directory.

To see what it inside this directory, use `ls`

## `ls` - List files inside the current directory

Nice, now you probably see the names of familiar folders and files,like Documents, Download, Pictures, etc. 

Let's say you want to create a new document inside the Documents folder. You can change your directory with the `cd` command

## `cd` - Change working directory

The formula for the `cd` command is simple: `cd <folder name>`

If you want to move into the Documents folder, then you would type: `cd Documents`

Great! Now you are in the documents folder. How do you create a new document or file? Use `touch`

## `touch` - Create a file

Think of this command as if you were an all-powerful being touching something into existence. That's basically what you are doing. 

Anyway, using `touch` is easy; the formula is `touch <filename.extension>`

If you want to create a text file called cool.text, then type: `touch cool.text`

You will need to write out the file extension here so don't forget that.

Go ahead, open up Finder and double check that cool.text is in the Documents folder. Better yet, have Finder open to Documents and watch the file get created in real time.

Maybe you like `cool.text` so much that you want to have two of them. Make a copy of it with `cp`

## `cp` - copy a file

The formula for `cp` is: `cp <file-to-copy> <name-of-copied-file`>

For example: `cp cool.text cool.text.2` creates a copy of `cool.text` that is called `cool.text.2` Use `ls` to prove it.


If you want to remove your creation, use `rm`

## `rm` - Remove a file

The formula here is the same: `rm <filename.extension>`

### Pro-tip: Use `tab` auto-complete to save on typing

Assumig you don't have other files that start with `cool` in your documents folder, type: `rm coo`, then hit `Tab`

This should auto-complete the filename such that it will say: `rm cool.text`. Then hit enter of course to remove the file.

Might as well delete `cool.text.2` while you're at it.

## `mkdir` - Create a folder

So you've created and removed a file, but now you want to create a folder to store things in.

The formula to do so is: `mkdir <folder name>`

If you want to make a folder called Coolness, type: `mkdir Coolness` 

Think this is a lame folder name? I agree. Let's remove it.

## `rm -r` - Remove a folder

STOP AND READ CAREFULLY.

`rm -r` is a powerful command. And we all know that with great power comes great responsibility. 

PLEASE ALWAYS TRIPLE CHECK BEFORE YOU USE THIS COMMAND. IF YOU ARE NOT CAREFUL, YOU COULD POTENTIALLY WIPE YOUR COMPUTER.

Here's why. That `-r` is a flag. A flag is basically a subcommand for the command you are already using. 

The `-r` command means `recursive`. This means that the command will delete the specified folder, and also everything that's inside of it. 

This is great if you want to remove a folder with a hundred files in it at once, but if by accident you used this command in the wrong directory, you could delete say, your Documents folder, and that would suck.

Let's not end on something sad and scary. Move on for some more pro tips.

## Some more pro tips: Using  `~ `,  `. `, and  `.. `

These weird litte symbols are probably ones I use most often. 

They are shortcuts to folders. And they can be used with all of the commands we just talked about (`ls`,`cd`,`touch`,`rm`,etc.) and more. Well not `pwd` actually, but everything else.

## Your Home Directory: `~`
Let's say you are deep into folders and sub-folders and you're running out of oxygen. If you want to quickly get back to your home directory, combine this guy with our old friend `cd` and type: `cd ~`

## Go back a directory: `..`

You're in the folder Documents/Coolness, but you're tryna ditch that lame folder. Type `cd ..` to go backwards a directory into the Documents folder. 

If you wanted to go back two folder levels, type: `cd ../..`, and just add another `/..` for every additional folder level you'd like to go back to.

## Reference the current directory: `.`

Earlier we used `ls` to list files in the current directory. An alternative way we could have done this is by using `ls .` 

Not so useful to add `.` in this case, but there are times you will use it. 


## Get used to using these commands. 
They are your best friends and it will become second nature to use them after not too long.

### And if you forget anything, use Google
It's definitely highly recommended to use Google to figure things out. Much better than wasting time trying random things until it works (or doesn't.)

# Congrats
You are now able to get around your computer without using your mouse. This is actually a really big achievement because these skills are foundational to everything else you will do. 


#### More commands if you want, but you don't need them right now
There are many more commands you can use, many of which are useful. You probably don't need to know any more at this point in the game, and should probably focus on getting familiar with the commands we just talked about first.

If you are tempted by curiousity however, there are a few things to know.

`man` is a command that tells you more about other commands. If you wanted to learn about all the flags for `ls`, type: `man ls`
You might find out that `ls -a` lets you see hidden files for example. 

If you want to see all of the commands out there and how to use them, try googling `list of shell commands` and have fun.







