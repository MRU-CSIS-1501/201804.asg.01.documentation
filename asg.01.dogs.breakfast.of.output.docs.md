# Assignment 01

## Challenge: Dogs Breakfast of Output

### Preamble

You'll be doing a **lot** of output to the console in this course (and when you code in general, no matter the language). Being comfortable with the different ways to get this done is important.

In Java, you're typically going to reach for `print` and `println` when you are doing simple output without formatting; when you need to do some kind of formatting - like setting field widths, rounding numbers to a certain number of decimal places, or adding grouping separators (like the **,** in **1,234**) you'll reach for `printf` (or `format`, which is equivalent).

This challenge just tosses a mish-mash of output tasks your way to start building your experience with output.

---

### What you're going to build

When you run this program, there is no user input; we just get console output:

**Expected Console Output**

<pre>
***** print and println using concatenation *****
The Algorithm March Reloaded: https://www.youtube.com/watch?v=jVMsHHFJX68

***** leading zeroes, width *****
0007
007
07
7

***** precision with strings *****
bur
burr
burro
burrow
burrows

***** alignment, width, more than one format specifier *****
  earth : 地  (tsuchi)
  water : 水  (mizu)
   fire : 火  (hi)
    air : 風  (kaze)

***** precision with numbers, comma grouping *****
666 six-packs of Trash Panda in Calgary:   $12,107.41
666 six-packs of Trash Panda in Vancouver: $10,558.43
 </pre>

> Commentary
>
> - Each section of output starts with a header (like `***** leading zeroes, width *****`)
> - There is a blank line between each section.

#### Instructions

You have been provided with the file `DogsBreakfastOfOutput.java`. It has a `run` method where you should add the code necessary to get the output look as expected.

Read the comments included in the file - if you don't, chances are you won't get full marks for this challenge.
