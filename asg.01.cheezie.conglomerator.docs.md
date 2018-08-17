# Assignment 01

## Challenge: Cheezies Conglomerator

### Preamble

I was eating some Cheezies&reg; the other day. They were so delicious that this assignment popped out.

Imagine that you're a particularly fastidious screenwriter who prides themselves on being numerically accurate in all that you do. You've been asked to write a screenplay for a "reimagining" of the film Frankenstein.

In the new film, the mad scientist creates, instead of a monster, a Device&reg; that can make Cheezies&reg; - given enough time, perhaps an infinite number of them.

Terrifying.

To profit from the Device&reg;, the mad scientist wishes to sell those Cheezies&reg;. Naturally, packaging is important.

The scientist comes up with a packaging system: mainly, have their trusted assistant (Igor, of course) stuff individual Cheezies&reg; into bags, then bags into boxes, and then boxes onto pallets.

- Each **bag** can hold _exactly_ 117 individual Cheezies&reg;.
- A **box** can hold 32 bags.
- A **pallet** can hold 12 boxes.

You haven't decided on exactly how many Cheezies&reg; to use yet..but by Galookum, the number of bags, boxes, and pallets in the script will be **accurate**.

---

### What you're going to build

You're going to make software that asks for the total number of Cheezies&reg; created by the Device&reg; and then spits back the riveting scene in the screenplay that involves Igor reporting the results of his inaugural packing.

**Example Run 1:**
(User input is shown in **bold**.)

<pre>
How many Cheezies® did The Device® create? <b>12231</b>

    MAD SCI
How many Cheezies® did The Device® create today, Igor?

    IGOR
12,231, master.

   MAD SCI
12,231?!?
Why...why that's (thinks furiously for a moment)...that's...

0 full pallets,
3 loose boxes,
8 loose bags, and
63 loose Cheezies® !

Excellent, Igor. That should keep those accursed peasants happy.
</pre>

**Example Run 2:**

<pre>
How many Cheezies® did The Device® create? <b>89973</b>

    MAD SCI
How many Cheezies® did The Device® create today, Igor?

    IGOR
89,973, master.

   MAD SCI
89,973?!?
Why...why that's (thinks furiously for a moment)...that's...

2 full pallets,
0 loose boxes,
1 loose bags, and
0 loose Cheezies® !

Excellent, Igor. That should keep those accursed peasants happy.
</pre>

#### Instructions

You have been provided with a class called `CheezieConglomerator`. It has 6 documented methods that are currently stubbed out :

1. `numPallets`
2. `totalNumBoxes`
3. `totalNumBags`
4. `numLooseBoxes`
5. `numLooseBags`
6. `numLooseCheezies`

To complete this challenge successfully, you **must**:

1. Code the 6 methods given to you so that they behave as documented.
   - Don't panic - each of these methods should be just a single line of code!
2. Complete the `run` method so that when the program is run, it behaves as shown in the examples above.
   - You **must** use the 6 methods provided in your final solution.
   - Further methods might be a good idea.

Look to the rubric for further guidance.
