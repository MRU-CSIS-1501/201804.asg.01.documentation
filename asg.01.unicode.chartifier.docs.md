# Assignment 01

## Challenge: Unicode Chartifier

### Before you begin

If you plan on doing much development for this assignment on your own laptop or home computer, make sure you download the font [DejaVu Sans Mono](https://www.fontsquirrel.com/fonts/dejavu-sans-mono) and use it as your font when working in KiTTY (Windows) or your terminal editor (Mac or Linux). This font has a much wider support of Unicode characters than the default fonts typically found.

If you are working in KiTTY, you will have the best luck in finding how to do this by searching for instructions online if you use **putty** instead of **kitty** in your search.

If you're on a Mac, you'll want to include the word **terminal** in your search.

---

### Preamble

So there are a **lot** of Unicode characters. They are arranged into "blocks" - you can see them all at the very wonderful [unicode-table.com](https://www.fileformat.info/info/unicode/block/index.htm).

(You may want to pop that link open and have the page handy before continuing.)

The very first block is the **Basic Latin** block - that's where the all the characters in the English alphabet, numbers, and basic punctuation marks live in relative peace and harmony.

See those entries in the **From** column? Like the **U+0000**? Those entries are examples of _Unicode code points_ - the underlying numbers that represent characters you see on a screen. (You might be wondering why some of the code points in the column have letters in them. It's because the numbers following the + are in base 16, not the base 10 we humans are used to. You'll see more of these base 16 numbers, called _hexadecimal numbers_, in COMP2531. For now, just accept that they exist and look weird.)

---

### What you're going to build

You're going to be making a program that asks the user for a Unicode code point in the form **U+xxxx** and then displays a chart showing the corresponding character at that code point, as well as the code points and characters immediately before and after the given one.

**Example Run 1**
(User input is shown in **bold**.)

<pre>
Unicode code point: <b>U+0057</b>
┏━━━━━━━━┳━━━━━━━━┳━━━━━━━━┓
┃ U+0056 ┃ U+0057 ┃ U+0058 ┃
┣━━━━━━━━╋━━━━━━━━╋━━━━━━━━┫
┃   V    ┃   W    ┃   X    ┃
┗━━━━━━━━┻━━━━━━━━┻━━━━━━━━┛
</pre>

> Commentary on Run 1
>
> - Note that the code point entered by the user becomes the middle entry in the table.

**Example Run 2**

<pre>
Unicode code point: <b>U+20A4</b>
┏━━━━━━━━┳━━━━━━━━┳━━━━━━━━┓
┃ U+20A3 ┃ U+20A4 ┃ U+20A5 ┃
┣━━━━━━━━╋━━━━━━━━╋━━━━━━━━┫
┃   ₣    ┃   ₤    ┃   ₥    ┃
┗━━━━━━━━┻━━━━━━━━┻━━━━━━━━┛
 </pre>

> Commentary on Run 2
>
> - Here we see that the code points are such that we're no longer displaying characters in the Basic Latin block.

**Example Run 3**

<pre>
Unicode code point: U+1F6A0
┏━━━━━━━━┳━━━━━━━━┳━━━━━━━━┓
┃ U+1F69F ┃ U+1F6A0 ┃ U+1F6A1 ┃
┣━━━━━━━━╋━━━━━━━━╋━━━━━━━━┫
┃       ┃       ┃       ┃
┗━━━━━━━━┻━━━━━━━━┻━━━━━━━━┛
 </pre>

> Commentary on Run 3
>
> - Here's what you see if you go into a block that your font can't represent - you get these lovely squares...your computer's way of saying "I don't know how the hell to display this character for you - here's a box for you instead".
> - Note that we've kinda messed up our table alignment because the number of characters in the code points is large. We're not going to worry about this ... but it goes to show you that there's **always** something that can go wrong when you're programming! Learning how to anticipate these problems in advance is a skill you will develop with experience.

#### Instructions

You have been provided with a class called `UnicodeChartifier`. It has a number of methods, 2 of which are stubbed out:

1.  `unicodeChar`
2.  `offsetCodePoint`

For full marks, you **must**:

1.  Code the 2 methods above so that they behave as documented.
    - You must use `String.format` in `offsetCodePoint`.
2.  Complete the `run` method so that when the program is run, it behaves as shown in the examples above.
    - You **must** use all of the provided methods (not just the stubbed ones) in your final solution.
    - You should try and make some other methods as well.
    - You must use `System.out.printf` at least once and `System.out.println` at least once.
    - You must use the `┃`character (U+2503) to draw the vertical pipes in these methods - don't use the `|` character found on the keyboard.

#### Things to ponder

- The user will enter a code point as a String...but how are you going to turn this into a number? You not only have to somehow get to the part of the String that's _after_ the `U+`, but then also somehow turn **that** into an integer....
- Working with `String.format` and `System.out.printf` will be weird at first. Be prepared to look things up in your text book or do some digging online to make things work properly.
