#Command Line

## Goals

- Learn about the command line
- Make a new directory
- Browse some directories on your computer
- Learn the commands `pwd`, `mkdir`, `ls`, `cd` and `man`

### Step 1
Open up a command line application on your computer. On Macs, this program is called Terminal. On Windows, you will be using the Git shell with `vagrant ssh`.

Type this in the terminal:


```bash
pwd
```

pwd means "print working directory". It shows you what *directory* you're currently in. Directories are also often called folders.

pwd can help orient you in the command line if you get lost somewhere in your computer.

### Step 2

Type this in the terminal:

```bash
mkdir railsbridge_ruby
```

mkdir means make directory. You use mkdir when you want to create a new directory.

The command line is just one way of manipulating the files on your computer. Try to find the new directory you created in Finder or Windows Explorer.

If you get an error saying the directory already exists, maybe someone did these steps on your computer before. Don't fret.

### Step 3

Type this in the terminal:

```bash
cd railsbridge_ruby
```

`cd` means change directory. You use cd when you want to move from the current directory into some other directory.

### Step 4

If you're on a Mac or Linux computer:

Type this in the terminal:

```bash
cd ~
```

`~` indicates your *home directory*, a directory owned by the account currently logged in to the computer. Your home directory might be something like `/home/sparklepants` (Linux) or `/Users/saucyfrank` (Mac)

Practice moving in and out of various directories. Remember that you can always get back to your home with `cd ~`.

### Step 5

Type this in the terminal:

```bash
ls
```

`ls` stands for *list*, and shows the contents of the current directory.

Since you moved back to your Home directory, you should see the newly-created railsbridge_ruby directory in the output of ls.

### Step 6

Type this in the terminal:

```bash
man ls
```

`man` stands for *manual* and shows you the documentation for a command. This can include various options used to run the command in different ways.

If you see a colon at the bottom of your terminal when viewing a man page, it means you're in a pager. Pagers are special programs for showing text that spans multiple pages. You can press the up and down arrows to page through the text, or type q to exit.

## Explanation

The command line is an essential tool for computer programmers. While daunting at first, it offers great flexibility in moving around your computer and manipulating files.

There are many, many, many more commands available on the command line than what we've seen here, but these are enough to get you going.

Command summary:
<table class="table">
  <thead>
    <th>Command</th>
    <th>Name</th>
    <th>Description</th>
  </thead>
  <tbody>
    <tr>
      <td>pwd</td>
      <td>print working directory </td>
      <td>print the full path to your current directory</td>
    </th>
    <tr>
      <td>ls</td>
      <td>list directory</td>
      <td>display the contents of the current directory </td>
    </th>
    <tr>
      <td>cd [directory] </td>
      <td>change directory</td>
      <td>make this directory the current directory</td>
    </th>
    <tr>
      <td>man [cmd]</td>
      <td>manual</td>
      <td>show the manual for this command. press 'q' to quit</td>
    </th>
</table>


## Next Step:

Go on to [irb](irb)
