---
title: "Understanding the Command Line"
seoTitle: "Master Command Line Basics"
seoDescription: "Master Bash with this guide, exploring Shell vs Kernel, CLI benefits, and key commands for files and directories"
datePublished: Tue Oct 03 2023 19:57:54 GMT+0000 (Coordinated Universal Time)
cuid: clnaqrxb6000009kve2nd2a9v
slug: understanding-the-command-line
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1696357690021/0e7e0b5c-7267-4240-a91a-bd25530a8c6b.jpeg
tags: unix, linux, bash, command-line, wemakedevs

---

### **In this article, we will understand a Unix-based command line, the Bash!**

### What are Shell and Kernel?

In any computing system, say we consider the Operating System as a "Pistachio".

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1696359302542/20469998-49cc-4176-b461-413b23f9b618.png align="center")

The core of the Operating System is called a **Kernel**. The Kernel has complete control over everything in the system and it facilitates interactions between hardware and software components.

And, the outermost layer of the Operating System is known as the **Shell**. It acts as an Interface between the user and the kernel. It allows a user to give commands to the kernel and receive responses from it.

A Shell can be a Graphical User Interface (GUI) such as the File Explorer or a Command Line Interface (CLI) such as **Bash**. The most common shell available on all Linux and Debian-based systems is BASH, aka Bourne Again Shell.

### Why Would You Use CLI over GUI?

The GUI was developed within the operating system as soon as the mouse became a new input device to operate the computer.

We should admit that GUI is **visually attractive and easily understood**. But, for some vital tasks, CLI is way more powerful.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1696359330714/50751cbb-c2da-4eea-8187-f5763576b7ce.png align="center")

Here, we would like to pick some points why you would use CLI over GUI.

1. **Less Resource** It is not a secret that the text-based program needs very few resources from your computer. This means that with CLI you can do similar tasks with minimum resources.
    
2. **High Precision** You can use a specific command to target specific destinations with ease. As long as you don’t type the wrong command, it will work like a charm. Once you learn the basics, writing syntax is not as hard as you might think.
    
3. **Repetitive Tasks Friendly** GUI has developed well over the years. But, the operating system may not give you all the menus and buttons to perform all tasks. One of the reasons is safety. This leaves you overwhelmed if you have to do repetitive tasks. For example, when you have to handle hundreds of files within a folder, CLI enables you to use a single command to automate the repetition easily.
    
4. **Powerful** Most operating systems today prevent you from messing up the system’s core process. Windows has system protection and MacOS has SIP (System Integrity Protection). You won’t be able to perform certain tasks that are system-protected. However, with CLI, you will have full control over your system.
    

While the GUI may seem appealing, CLI is light, powerful and straightforward.

Source: [https://www.hostinger.in/tutorials/what-is-cli](https://www.hostinger.in/tutorials/what-is-cli)

### Learn enough command line to be dangerous

To understand the command syntax in Bash, let’s learn from these examples:

# `Basics`

<table><tbody><tr><td colspan="1" rowspan="1"><p><strong>Command</strong></p></td><td colspan="1" rowspan="1"><p><strong>Description</strong></p></td><td colspan="1" rowspan="1"><p><strong>Example</strong></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>echo &lt;string&gt;</code></p></td><td colspan="1" rowspan="1"><p>Print string to screen</p></td><td colspan="1" rowspan="1"><p><code>$ echo hello</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>man &lt;command&gt;</code></p></td><td colspan="1" rowspan="1"><p>Display manual page for command</p></td><td colspan="1" rowspan="1"><p><code>$ man mkdir</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>⌃C</code></p></td><td colspan="1" rowspan="1"><p>Get out of trouble</p></td><td colspan="1" rowspan="1"><p><code>$ tail ⌃C</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>⌃A</code></p></td><td colspan="1" rowspan="1"><p>Move to beginning of line</p></td><td colspan="1" rowspan="1"><p></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>⌃E</code></p></td><td colspan="1" rowspan="1"><p>Move to end of line</p></td><td colspan="1" rowspan="1"><p></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>⌃U</code></p></td><td colspan="1" rowspan="1"><p>Delete to beginning of line</p></td><td colspan="1" rowspan="1"><p></p></td></tr><tr><td colspan="1" rowspan="1"><p>Option-click</p></td><td colspan="1" rowspan="1"><p>Move cursor to location clicked</p></td><td colspan="1" rowspan="1"><p></p></td></tr><tr><td colspan="1" rowspan="1"><p>Up &amp; down arrow</p></td><td colspan="1" rowspan="1"><p>Scroll through previous commands</p></td><td colspan="1" rowspan="1"><p></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>clear</code>&nbsp;or&nbsp;<code>⌃L</code></p></td><td colspan="1" rowspan="1"><p>Clear screen</p></td><td colspan="1" rowspan="1"><p><code>$ clear</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>exit</code>&nbsp;or&nbsp;<code>⌃D</code></p></td><td colspan="1" rowspan="1"><p>Exit terminal</p></td><td colspan="1" rowspan="1"><p><code>$ exit</code></p></td></tr></tbody></table>

Note:

* On git bash you can use **&lt;command&gt; —help** instead of the **man &lt;command&gt;**
    
* The ***Alt key*** acts as an ***option key*** on ***Windows*** keyboards
    

# `Manipulating Files`

<table><tbody><tr><td colspan="1" rowspan="1"><p><strong>Command</strong></p></td><td colspan="1" rowspan="1"><p><strong>Description</strong></p></td><td colspan="1" rowspan="1"><p><strong>Example</strong></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>&gt;</code></p></td><td colspan="1" rowspan="1"><p>Redirect output to filename</p></td><td colspan="1" rowspan="1"><p><code>$ echo foo &gt; foo.txt</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>&gt;&gt;</code></p></td><td colspan="1" rowspan="1"><p>Append output to filename</p></td><td colspan="1" rowspan="1"><p><code>$ echo bar &gt;&gt; foo.txt</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>cat &lt;file&gt;</code></p></td><td colspan="1" rowspan="1"><p>Print contents of file to screen</p></td><td colspan="1" rowspan="1"><p><code>$ cat hello.txt</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>diff &lt;f1&gt; &lt;f2&gt;</code></p></td><td colspan="1" rowspan="1"><p>Diff files 1 &amp; 2</p></td><td colspan="1" rowspan="1"><p><code>$ diff foo.txt bar.txt</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>ls</code></p></td><td colspan="1" rowspan="1"><p>List directory or file</p></td><td colspan="1" rowspan="1"><p><code>$ ls hello.txt</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>ls -l</code></p></td><td colspan="1" rowspan="1"><p>List long form</p></td><td colspan="1" rowspan="1"><p><code>$ ls -l hello.txt</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>ls -rtl</code></p></td><td colspan="1" rowspan="1"><p>Long by reverse modification time</p></td><td colspan="1" rowspan="1"><p><code>$ ls -rtl</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>ls -a</code></p></td><td colspan="1" rowspan="1"><p>List all (including hidden)</p></td><td colspan="1" rowspan="1"><p><code>$ ls -a</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>touch &lt;file&gt;</code></p></td><td colspan="1" rowspan="1"><p>Create an empty file</p></td><td colspan="1" rowspan="1"><p><code>$ touch foo</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>mv &lt;old&gt; &lt;new&gt;</code></p></td><td colspan="1" rowspan="1"><p>Rename (move) from old to new</p></td><td colspan="1" rowspan="1"><p><code>$ mv foo bar</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>cp &lt;old&gt; &lt;new&gt;</code></p></td><td colspan="1" rowspan="1"><p>Copy old to new</p></td><td colspan="1" rowspan="1"><p><code>$ cp foo bar</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>rm &lt;file&gt;</code></p></td><td colspan="1" rowspan="1"><p>Remove (delete) file</p></td><td colspan="1" rowspan="1"><p><code>$ rm foo</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>rm -f &lt;file&gt;</code></p></td><td colspan="1" rowspan="1"><p>Force-remove file</p></td><td colspan="1" rowspan="1"><p><code>$ rm -f bar</code></p></td></tr></tbody></table>

Note:

* The cat command can take multiple arguments, to combine several text files into a single file `cat file1 file2 file3 > newfile` If you want to add one or more files to an existing document, use `>>`
    
* When there is no diff between two files, diff simply outputs nothing
    
* By the way, `-rtl` is the commonly used compact form, but you can also pass the options individually, like this: `$ ls -r -t -l`. In addition, their order is irrelevant, so typing ls `-trl` gives the same result
    
* Using the `-h` (”human-readable”) option to `ls`, lists the long form of the file with a human-readable byte count (in kilobytes)
    
* Suppose you wanted to list the files and directories using human-readable byte counts, all, by reverse time-sorted long-form: `ls -rtlh`
    

# `Directories`

<table><tbody><tr><td colspan="1" rowspan="1"><p><strong>Command</strong></p></td><td colspan="1" rowspan="1"><p><strong>Description</strong></p></td><td colspan="1" rowspan="1"><p><strong>Example</strong></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>mkdir &lt;name&gt;</code></p></td><td colspan="1" rowspan="1"><p>Make directory with name</p></td><td colspan="1" rowspan="1"><p><code>$ mkdir foo</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>pwd</code></p></td><td colspan="1" rowspan="1"><p>Print working directory</p></td><td colspan="1" rowspan="1"><p><code>$ pwd</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>cd &lt;dir&gt;</code></p></td><td colspan="1" rowspan="1"><p>Change to &lt;dir&gt;</p></td><td colspan="1" rowspan="1"><p><code>$ cd foo/</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>cd ~/&lt;dir&gt;</code></p></td><td colspan="1" rowspan="1"><p>cd relative to home</p></td><td colspan="1" rowspan="1"><p><code>$ cd ~/foo/</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>cd</code></p></td><td colspan="1" rowspan="1"><p>Change to home directory</p></td><td colspan="1" rowspan="1"><p><code>$ cd</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>cd -</code></p></td><td colspan="1" rowspan="1"><p>Change to previous directory</p></td><td colspan="1" rowspan="1"><p><code>$ cd &amp;&amp; pwd &amp;&amp; cd -</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>.</code></p></td><td colspan="1" rowspan="1"><p>The current directory</p></td><td colspan="1" rowspan="1"><p><code>$ cp ~/foo.txt .</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>..</code></p></td><td colspan="1" rowspan="1"><p>One directory up</p></td><td colspan="1" rowspan="1"><p><code>$ cd ..</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>find</code></p></td><td colspan="1" rowspan="1"><p>Find files &amp; directories</p></td><td colspan="1" rowspan="1"><p><code>$ find . -name foo*.*</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>cp -r &lt;old&gt; &lt;new&gt;</code></p></td><td colspan="1" rowspan="1"><p>Copy recursively</p></td><td colspan="1" rowspan="1"><p><code>$ cp -r ~/foo .</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>rmdir &lt;dir&gt;</code></p></td><td colspan="1" rowspan="1"><p>Remove (empty) dir</p></td><td colspan="1" rowspan="1"><p><code>$ rmdir foo/</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>rm -rf &lt;dir&gt;</code></p></td><td colspan="1" rowspan="1"><p>Remove dir &amp; contents</p></td><td colspan="1" rowspan="1"><p><code>$ rm -rf foo/</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>grep -ri &lt;string&gt; &lt;dir&gt;</code></p></td><td colspan="1" rowspan="1"><p>Grep recursively (case-insensitive)</p></td><td colspan="1" rowspan="1"><p><code>$ grep -ri foo bar/</code></p></td></tr></tbody></table>

Note:

* The tilde (~) is a Linux "shortcut" to denote a user's home directory. As a result, the two paths shown are identical: `/Users/sabhi/foo/projects` is the same as `~/foo/projects`
    
* To make the directory foo and, within it, the directory bar (i.e., ~/foo/bar) with a single command: `mkdir -p ~/foo/bar`. Also, `mkdir` accepts multiple path arguments: `mkdir -p -- a/foo b/bar a/baz`
    
* If you want to copy only the files, be explicit using the star operator, as in: `$ cp ../text_files/* .`
    
* The command `rm -rf /` is unbelievably dangerous, and you should never type it into a terminal window, not even as a joke.
    

# `Inspecting Files`

<table><tbody><tr><td colspan="1" rowspan="1"><p><strong>Command</strong></p></td><td colspan="1" rowspan="1"><p><strong>Description</strong></p></td><td colspan="1" rowspan="1"><p><strong>Example</strong></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>curl</code></p></td><td colspan="1" rowspan="1"><p>Interact with URLs</p></td><td colspan="1" rowspan="1"><p><code>$ curl -O example.com</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>which</code></p></td><td colspan="1" rowspan="1"><p>Locate a program on the path</p></td><td colspan="1" rowspan="1"><p><code>$ which curl</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>head &lt;file&gt;</code></p></td><td colspan="1" rowspan="1"><p>Display first part of file</p></td><td colspan="1" rowspan="1"><p><code>$ head foo</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>tail &lt;file&gt;</code></p></td><td colspan="1" rowspan="1"><p>Display last part of file</p></td><td colspan="1" rowspan="1"><p><code>$ tail bar</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>wc &lt;file&gt;</code></p></td><td colspan="1" rowspan="1"><p>Count lines, words, bytes</p></td><td colspan="1" rowspan="1"><p><code>$ wc foo</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>cmd1 | cmd2</code></p></td><td colspan="1" rowspan="1"><p>Pipe cmd1 to cmd2</p></td><td colspan="1" rowspan="1"><p><code>$ head foo | wc</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>less &lt;file&gt;</code></p></td><td colspan="1" rowspan="1"><p>View file contents interactively</p></td><td colspan="1" rowspan="1"><p><code>$ less foo</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>grep &lt;string&gt; &lt;file&gt;</code></p></td><td colspan="1" rowspan="1"><p>Find string in file</p></td><td colspan="1" rowspan="1"><p><code>$ grep foo bar.txt</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>grep -i &lt;string&gt; &lt;file&gt;</code></p></td><td colspan="1" rowspan="1"><p>Find case-insensitively</p></td><td colspan="1" rowspan="1"><p><code>$ grep -i foo bar.txt</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>ps</code></p></td><td colspan="1" rowspan="1"><p>Show processes</p></td><td colspan="1" rowspan="1"><p><code>$ ps aux</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>top</code></p></td><td colspan="1" rowspan="1"><p>Show processes (sorted)</p></td><td colspan="1" rowspan="1"><p><code>$ top</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>kill -15 &lt;pid&gt;</code></p></td><td colspan="1" rowspan="1"><p>Kill a process</p></td><td colspan="1" rowspan="1"><p><code>$ kill -9 24601</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>pkill -15 -f &lt;name&gt;</code></p></td><td colspan="1" rowspan="1"><p>Kill matching processes</p></td><td colspan="1" rowspan="1"><p><code>$ pkill -9 -f spring</code></p></td></tr></tbody></table>

Note:

* Downloading a file: We can download a file from the Internet using the powerful curl utility: `curl -OL <https://cdn.learnenough.com/sonnets.txt>`
    
* By default, the `head` command shows the first 10 lines of the file. Similarly, `tail` shows the last 10 lines of the file
    
* To look at the first n lines (say 25) of the file: `head -n 25 <filename>`
    
* Using the `less` Command: Less is an awesome Linux command utility for viewing text files. The most important `less` commands:
    
    <table><tbody><tr><td colspan="1" rowspan="1"><p><strong>Command</strong></p></td><td colspan="1" rowspan="1"><p><strong>Description</strong></p></td><td colspan="1" rowspan="1"><p><strong>Example</strong></p></td></tr><tr><td colspan="1" rowspan="1"><p>Up &amp; down arrow</p></td><td colspan="1" rowspan="1"><p>Move up or down one line</p></td><td colspan="1" rowspan="1"><p></p></td></tr><tr><td colspan="1" rowspan="1"><p>Spacebar</p></td><td colspan="1" rowspan="1"><p>Move forward one page</p></td><td colspan="1" rowspan="1"><p></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>⌃F</code></p></td><td colspan="1" rowspan="1"><p>Move forward one page</p></td><td colspan="1" rowspan="1"><p></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>⌃B</code></p></td><td colspan="1" rowspan="1"><p>Move back one page</p></td><td colspan="1" rowspan="1"><p></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>G</code></p></td><td colspan="1" rowspan="1"><p>Move to end of file</p></td><td colspan="1" rowspan="1"><p></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>IG</code></p></td><td colspan="1" rowspan="1"><p>Move to beginning of file</p></td><td colspan="1" rowspan="1"><p></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>/&lt;string&gt;</code></p></td><td colspan="1" rowspan="1"><p>Search file for string</p></td><td colspan="1" rowspan="1"><p><code>$ /rose</code></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>n</code></p></td><td colspan="1" rowspan="1"><p>Move to next search result</p></td><td colspan="1" rowspan="1"><p></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>N</code></p></td><td colspan="1" rowspan="1"><p>Move to previous search result</p></td><td colspan="1" rowspan="1"><p></p></td></tr><tr><td colspan="1" rowspan="1"><p><code>q</code></p></td><td colspan="1" rowspan="1"><p>Quit less</p></td><td colspan="1" rowspan="1"><p></p></td></tr></tbody></table>
    

# `An Extra Bit: Repeating previous commands:`

So far, we’ve used the up-arrow key to retrieve (and possibly edit) previous commands, but this isn’t the only possibility.

An even quicker way to find and immediately run a previous command involves using the exclamation point `!` which in the context of software development is usually pronounced “**bang**”.

To run the previous command exactly as written, we can use `!!` “**bang bang**”:

```bash
$ cat hello.txt
Hello world ..!
$ !!
cat hello.txt
Hello world ..!
```

A closely related usage is “bang” followed by some number of characters, which runs the last command that starts with those characters.

For example, to run the last curl command, we could type this: `$ !curl`

This would save us the trouble of typing out the options, the URL, etc. Depending on our history of commands, the even terser !cu or !c would work as well.

A second and incredibly powerful technique is `reverse-i-search`**.**

**CTRL+R** activates `reverse-i-search`, which provides a nice search area, giving you an easier way to navigate through your history.

```bash
$ ⌃R
(reverse-i-search)`': curl
```

Check this article for more info: [*Bash bang commands: A must-know trick for the Linux command line | Enable Sysadmin (*](https://www.redhat.com/sysadmin/bash-bang-commands)[*redhat.com*](http://redhat.com)[*)*](https://www.redhat.com/sysadmin/bash-bang-commands)

## `Congratulations`!🎉

You’ve officially learned enough command line to be dangerous.

I recommend following the [Learn Enough](https://www.learnenough.com/command-line-tutorial/basics)™, as it represents the shortest path to technical proficiency and software development skills.

References: [*Learn Enough Command Line to Be Dangerous*](https://www.learnenough.com/command-line-tutorial) by [Michael Hartl](https://www.learnenough.com/command-line#author) is an introduction to the Unix command line for complete beginners.