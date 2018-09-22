# Assignment 01

**DUE: September 27, 2018 @ 5:00PM**

**WEIGHT: 4%**

**ANY QUESTIONS?** Please post any questions to [Piazza](https://piazza.com/class/jm9cg39jrr21zs?cid=9#), ideally in the **assignment1** folder.

## A few WARNINGS

- For most of you, this is your first programming assignment - and even if it's not, it's _extremely_ likely that it _is_ your first time to be working in a command line environment. Because of this, you will likely struggle mightily with this assignment. Budget your time wisely.

- You will likely be frustrated with some of the quirks of working in Emacs. Even things most consider to be easy tasks - like copy and pasting - are going to require you to learn some new skills. Persevere. It will get easier - **but only with practice**.

- You might be dismayed at the amount of text in the challenge descriptions below. It's there for a reason. Skim at your peril.

- You don't have to do the challenges in the order presented. Please feel free to cherry pick. That being said, the _Dog's Breakfast of Output_ is an easier place to start. Probably.

## Before you begin

If you plan on doing much development for this assignment on your own laptop or home computer, make sure you download the font [DejaVu Sans Mono](https://www.fontsquirrel.com/fonts/dejavu-sans-mono) and use it as your font when working in KiTTY (Windows) or your terminal editor (Mac or Linux). This font has a much wider support of Unicode characters than the default fonts typically found.

If you are working in KiTTY, you will have the best luck in finding how to do this by searching for instructions online if you use **putty** instead of **kitty** in your search.

If you're on a Mac, you'll want to include the word **terminal** in your search.

## Getting the starting code

You will be adding code to source files already created for you.

Please copy the directory `/users/library/csis/comp1501/assignments/1.asg.jpratt` to your home directory.

If you don't know how to do this, you can use the Linux command reference given to you in lab-00, or Google away.

## How to check your work

If you want to check whether your code is _behaving as expected_, you can run the command **make tests** from the directory of the challenge you're
working on.

> Just because the given tests run green does **not** mean everything is
> fine - we've only included a handful of the test data we will use to
> actually mark your assignments for correctness! You can add your own test
> data to the csv files in the `tests/data` directory; just add additional
> rows to the data already there.

If you want to see whether your code is _following the coding standards for this course_, you can run the command **make style -i** from the directory
of the challenge you're working on.

> There is some overlap between the two tools used to do this task, so
> you may notice some warnings are repeated between the two tools. If you
> don't understand any of the warnings (they **can** be a little opaque),
> please talk to one of the IAs or your instructor.

---

### Things you'll see in this assignment

- constants
- variables
- parameters
- methods
- `Scanner` (for input from keyboard)
- `System.out.println`
- value-returning methods (a.k.a. functions)
- `String.format`
- `System.out.format/printf`
- integer division (`/`) and integer remainder (`%`)

### Things you'll do in this assignment

- compile your code
- fix syntax and logic errors
- debug
- read documentation
- read other people's code
- run automated tests
- run static code checkers
- break problems into small chunks (a.k.a. functional decomposition)
- get keyboard input

### Collateral Learning Opportunities

- installing a new font
- installing Kitty (or using Terminal on a Mac)
