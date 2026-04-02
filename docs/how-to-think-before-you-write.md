# How to Think Before You Write a Program

> A Practical Problem-Solving Workflow for Programming Logic


## Why this document exists

In this subject, you are **not learning a programming language yet**.

You are learning **how to think like a problem solver**, and how to communicate that thinking using:

* IPO charts
* Pseudocode
* Flowcharts

Many students try to jump straight from a question to a solution. That approach might seem to work when using AI or copying examples, but it **does not build real understanding**, and it will not support you in tests or exams.

This document gives you a **repeatable workflow** that you should follow every time you are given a programming problem — in class, in homework, and in assessments.

---

## ⟡ Quick Start — What You Do When You Get a Question

If you feel unsure where to begin, follow this checklist:

1. **Do NOT write code**
2. Identify:

   * GIVEN information
   * INPUT required
   * OUTPUT required
3. Draw a simple **IPO chart**
4. Write the solution in **plain English steps**
5. Convert those steps into **pseudocode**
6. Represent the logic using a **flowchart**

> If you skip these steps, you are guessing — not solving.

You may not need to read this entire document every time.
Use it as a **reference guide** — return to the section you need when you need it.

---

## Part 1: The Foundation — How to Solve Any Problem

Before computers existed, people solved problems using a structured process. Programming does **not replace** these steps. It **formalises** them.

### The Six Steps of Problem Solving

**Step 1: Identify the Problem (Clearly Define the Problem)**

Before a solution can be found, the problem must be understood. What exactly needs to be solved? Extract and frame the specific goal. Without a clear definition, problem solving cannot begin.

---

**Step 2: Understand the Problem (Context and Constraints)**

Consider the context:

* For human users: what do they already know? What assumptions might they make?
* For computers: what are the rules, limitations, and structure of the environment?

Also consider your own understanding. You cannot design a solution unless you clearly comprehend the problem yourself.

> Analogy: Giving directions to someone unfamiliar with an area. Your instructions will differ based on their knowledge.

---

**Step 3: Identify Alternative Ways to Solve the Problem**

Think of multiple possible approaches. Draw from your experience, discuss with peers, or review similar examples. Each option should be logical and realistic within the given context.

---

**Step 4: Select the Most Suitable Solution**

Evaluate your options using ideas such as:

* Simplicity
* Clarity
* Efficiency
* Fit for the problem

Choose the approach that best balances these factors.

---

**Step 5: Outline the Solution as a Set of Instructions**

Break your solution into clear, step-by-step instructions. This becomes your **algorithm**.

If the solution is for a computer, the instructions must be precise, ordered, and unambiguous.

---

**Step 6: Test and Evaluate the Solution**

Apply your solution and review the outcome:

* Does it solve the original problem?
* Does it behave as expected?

If not, revisit earlier steps. This is a normal part of problem solving.

---

## Part 2: The Same Idea, Applied to Computers

When solving problems for a computer, we follow the same thinking process in a more structured way.

### The Program Development Cycle

**Step 1: Understand the Problem**

Identify user needs, clarify requirements, and define the scope. A strong solution begins with a clear understanding.

---

**Step 2: Plan the Logic**

Use tools such as:

* IPO charts
* Pseudocode
* Flowcharts

Break the solution into logical parts. You may also use trace tables or desk-checking to simulate the program before writing code.

---

**Step 3: Code the Program**

Translate your planned logic into a programming language. Good planning reduces errors and makes this step easier.

---

**Step 4: Translate into Machine Language**

Use a compiler or interpreter. Fix any syntax errors that arise.

---

**Step 5: Test the Program**

Use different inputs:

* Normal cases
* Edge cases
* Unexpected values

Correct any logic errors.

---

**Step 6: Put the Program into Production**

The program is used in a real-world environment.

---

**Step 7: Maintain the Program**

Programs evolve over time. Clear structure and comments make updates easier.

> This cycle is repeated as needed. Development is an iterative process.

---

## Part 3: The IPO Model — Your Anchor for Every Program

Every program follows the same structure.

### IPO = Input → Processing → Output

This is **not optional**. It is the foundation of all programming logic.

| Component      | Description                                                    |
| -------------- | -------------------------------------------------------------- |
| **Input**      | Data required (user input, files, sensors)                     |
| **Processing** | Steps that transform the data (calculations, decisions, loops) |
| **Output**     | The final result (display, file, system use)                   |

---

### ✔ IPO Check

Before moving on, ask yourself:

* Can I clearly list all inputs?
* Do I know exactly what must be output?
* Can I describe the processing in simple terms?

If not, you likely do not fully understand the problem yet.
Pause here and refine your thinking before continuing.

---

## Part 4: The Programming Logic Workflow (Follow This Every Time)

This is the core process you should apply to every problem.

---

### Step 1: Read the Question Without Thinking About Code

Do not think about `if`, loops, or formulas yet.

Ask:

| Question               | What you are identifying  |
| ---------------------- | ------------------------- |
| What is GIVEN?         | Information already known |
| What must be PROVIDED? | User input                |
| What must be PRODUCED? | Output                    |

If you immediately start thinking about code, pause and reread the question.

---

### Step 2: Extract IPO from the Question

Create a simple IPO chart:

```
INPUT
• …

PROCESS
• …

OUTPUT
• …
```

This step slows you down and helps prevent guessing.

---

### Step 3: Identify the Allowed Logical Structure

Each chapter introduces specific logic:

| Chapter | Allowed Logic                |
| ------- | ---------------------------- |
| Ch 4    | Sequential only              |
| Ch 5    | Sequential + Decision        |
| Ch 6    | Sequential + Decision + Loop |

Ask:

> “What logic am I expected to use here?”

**Key rule:**
If the logic has not been introduced yet, you must simulate it using simpler steps.

---

### Step 4: Rewrite the Solution in Plain English Steps

Describe the solution as simple actions:

* Receive input
* Perform calculation
* Update value
* Display result

If you cannot explain your solution in plain English, you are not ready to write pseudocode yet.

---

### Step 5: Convert Plain English into Pseudocode

Translate each step:

* One instruction per line
* No hidden logic
* No shortcuts

Your pseudocode should read like a clear set of instructions.

---

### Step 6: Use the Flowchart to Prove Your Logic

A flowchart is not decoration. It demonstrates:

* Order of execution
* Decision paths
* Repetition

Each pseudocode step should appear in the flowchart in the same order.

---

## ⟡ Using AI the Right Way

AI can be a useful tool — but only **after you have done the thinking**.

**Appropriate use:**

* You have completed your IPO
* You have written your own steps
* You are unsure how to express something in pseudocode

**Inappropriate use:**

* Asking for a full solution immediately
* Copying answers without understanding
* Skipping the planning process

> If you skip the thinking, you are training yourself to depend on AI rather than developing your own problem-solving ability.

---

## Part 5: Applying the Workflow — Three Complete Examples

The following examples show the workflow in action. For each question, you will see:
1. The question as given
2. The IPO extraction
3. The plain English steps
4. The final pseudocode

Follow along. Then apply the same process to your own homework.

---

### Example 1: Sequential Logic — Coin Change

**The Question**

Develop a solution that would:
a. Return the fewest coins in change from a purchase of under one rand. (Include 1c, 2c, 5c, 10c, 20c, and 50c coins in your solution.)

Example:
```
purchase 63c
change 37c

coins 
1 - 20c
1 - 10c
1 - 5c
1 - 2c
```

b. Develop a solution that would return the fewest notes (include our current set of South African notes used) and coins for a purchase under R100.

---

**Step 1: Read Without Code (Given, Provided, Produced)**

| Given | Provided | Produced |
|-------|----------|----------|
| Coin denominations (1c,2c,5c,10c,20c,50c) | Purchase amount (cents) | Number of 50c coins |
| Purchase is under 1 rand (100 cents) | | Number of 20c coins |
| | | Number of 10c coins |
| | | Number of 5c coins |
| | | Number of 2c coins |
| | | Number of 1c coins |

---

**Step 2: IPO Chart**

    INPUT
    • purchase amount (cents)

    PROCESS
    • calculate change = 100 - purchase
    • determine number of 50c coins (integer division)
    • subtract their value from change
    • determine number of 20c coins
    • subtract their value from change
    • continue for 10c, 5c, 2c, 1c

    OUTPUT
    • number of 50c coins
    • number of 20c coins
    • number of 10c coins
    • number of 5c coins
    • number of 2c coins
    • number of 1c coins

    No logic yet. No decisions yet. No loops yet. Just what exists.

---

**Step 3: Identify Allowed Logic**

This is Chapter 4 → **Sequential only**.

Key insight: Sequential logic means **every step happens**. Every coin type must be considered. Even zero results must be shown. Nothing is skipped.

---

**Step 4: Plain English Steps**

The program must:

1. Receive the purchase amount
2. Calculate the change (100 - purchase)
3. Determine how many 50c coins can be given
4. Subtract their value from the change
5. Determine how many 20c coins can be given
6. Subtract their value from the change
7. Continue for 10c, 5c, 2c, and 1c
8. Display **every coin type**, even if zero

---

**Step 5: Pseudocode**

```
0. Start
1. Declarations
      num intAmount
      num intChange
      num int50c
      num int20c
      num int10c
      num int5c
      num int2c
      num int1c

2.    output "Enter the amount you have purchased for under R1"
3.    input intAmount

4.    intChange = 100 - intAmount

5.    int50c = intChange \ 50
6.    intChange = intChange - (int50c * 50)

7.    int20c = intChange \ 20
8.    intChange = intChange - (int20c * 20)

9.    int10c = intChange \ 10
10.   intChange = intChange - (int10c * 10)

11.   int5c = intChange \ 5
12.   intChange = intChange - (int5c * 5)

13.   int2c = intChange \ 2
14.   intChange = intChange - (int2c * 2)

15.   int1c = intChange \ 1

16.   output "coins (to hand out for the change)"
17.   output int50c + " - 50c "
18.   output int20c + " - 20c "
19.   output int10c + " - 10c "
20.   output int5c + " - 5c "
21.   output int2c + " - 2c "
22.   output int1c + " - 1c "
23. Stop
```

---

**Step 6: Flowchart**

(To be drawn by you — each pseudocode line becomes a flowchart symbol in the same order.)

---

### Example 2: Decision Logic — Wholesale vs Retail Buyer

**The Question**

OG Floral's sells flowers to wholesale and retail buyers. The wholesale buyer needs a purchase number to buy at no tax and to receive discounts. The retail buyer pays 6% tax. Discounts for wholesale buyers:

| Amount | Discount |
|--------|----------|
| < R1000 | 2% |
| >= R1000 AND < R2500 | 5% |
| >= R2500 | 10% |

Develop the solution using straight‑through logic (separate sequential if...then statements) **and** using nested if...then statements. Output the amount the buyer is expected to pay.

---

**Step 1: Read Without Code (Given, Provided, Produced)**

| Given | Provided | Produced |
|-------|----------|----------|
| Discount brackets and percentages | Purchase amount | Final amount payable |
| Tax rate for retail (6%) | Resale number (or 0 if none) | |
| No tax for wholesale | | |

---

**Step 2: IPO Chart**

    INPUT
    • purchase amount
    • resale number (0 = retail, other = wholesale)

    PROCESS
    • if wholesale (resale number ≠ 0):
        - apply discount based on amount bracket
        - no tax
      else (retail):
        - add 6% tax
        - no discount

    OUTPUT
    • final amount payable

---

**Step 3: Identify Allowed Logic**

Chapter 5 → Sequential + Decision allowed.

---

**Step 4: Plain English Steps**

1. Receive purchase amount
2. Receive resale number
3. If resale number is not zero (wholesale):
   - If amount < 1000, discount = 2%
   - Else if amount < 2500, discount = 5%
   - Else discount = 10%
   - Final amount = amount - discount
4. Else (retail):
   - Final amount = amount + (amount × 6%)
5. Output final amount

---

**Step 5: Pseudocode — Two Versions**

**Version 1: Straight‑through logic (separate if statements)**

```
0. Start
1. Declarations
      num intResaleNumber = 0
      num fltAmount
      num fltFinalAmount

2.    output "Enter the amount that you are purchasing for "
3.    input fltAmount

4.    output "Are you a wholesale buyer? Please enter your resale number or 0"
5.    input intResaleNumber

6.    if intResaleNumber <> 0 then
         if fltAmount < 1000 then
            fltFinalAmount = fltAmount - (fltAmount * 0.02)
         endif
         if (fltAmount >= 1000) AND (fltAmount < 2500) then
            fltFinalAmount = fltAmount - (fltAmount * 0.05)
         endif
         if fltAmount >= 2500 then
            fltFinalAmount = fltAmount - (fltAmount * 0.1)
         endif
      else
         fltFinalAmount = fltAmount + (fltAmount * 0.06)
      endif

7.    output "The final amount payable R" + fltFinalAmount
8. Stop
```

**Version 2: Nested if‑then‑else (positive logic)**

```
0. Start
1. Declarations
      num intResaleNumber
      num fltAmount
      num fltFinalAmount

2.    output "Enter the amount that you are purchasing for "
3.    input fltAmount

4.    output "Are you a wholesale buyer? Please enter your resale number or 0"
5.    input intResaleNumber

6.    if intResaleNumber <> 0 then
         if fltAmount < 1000 then
            fltFinalAmount = fltAmount - (fltAmount * 0.02)
         else
            if fltAmount < 2500 then
               fltFinalAmount = fltAmount - (fltAmount * 0.05)
            else
               fltFinalAmount = fltAmount - (fltAmount * 0.1)
            endif
         endif
      else
         fltFinalAmount = fltAmount + (fltAmount * 0.06)
      endif

7.    output "The final amount payable R" + fltFinalAmount
8. Stop
```

**Key takeaway:** Both answers are correct because the conditions are mutually exclusive, but the structure changes readability and control flow. This is where thinking beats AI — AI rarely explains *why* one style is chosen over another.

---

### Example 3: Loop Logic — Loan Repayment

**The Question**

Create a program to accept from the user a loan amount and the repayment percentage value expected to be paid back for the loan. Print out the number of months it would take to pay back the loan.

---

**Step 1: Read Without Code (Given, Provided, Produced)**

| Given | Provided | Produced |
|-------|----------|----------|
| None (no constants given) | Loan amount | Number of months to repay |
| | Repayment percentage (e.g., 5% of remaining balance per month) | |

---

**Step 2: IPO Chart**

    INPUT
    • loan amount
    • repayment percentage (as a percentage, e.g., 5 for 5%)

    PROCESS
    • initialise month counter to 0
    • while loan balance > 0:
        - calculate repayment amount = balance × (percentage / 100)
        - subtract repayment from balance
        - increment month counter
        - (if repayment would exceed balance, just pay off remaining balance)

    OUTPUT
    • number of months

---

**Step 3: Identify Allowed Logic**

Chapter 6 → Sequential + Decision + Loop allowed.

---

**Step 4: Plain English Steps**

1. Receive loan amount
2. Receive repayment percentage
3. Set month count to 0
4. While loan balance is greater than 0:
   - Calculate repayment = balance × (percentage ÷ 100)
   - Subtract repayment from balance
   - Add 1 to month count
   - (If balance becomes negative, treat as 0 — the loan is paid)
5. Output month count

---

**Step 5: Pseudocode**

```
0. Start
1. Declarations
      num fltLoanBalance
      num fltRepaymentPercent
      num fltRepaymentAmount
      num intMonths = 0

2.    output "Enter the loan amount: "
3.    input fltLoanBalance

4.    output "Enter the repayment percentage (e.g., 5 for 5%): "
5.    input fltRepaymentPercent

6.    while fltLoanBalance > 0 do
         fltRepaymentAmount = fltLoanBalance * (fltRepaymentPercent / 100)
         fltLoanBalance = fltLoanBalance - fltRepaymentAmount
         intMonths = intMonths + 1
      endwhile
7.    output "Months to repay: " + intMonths
8. Stop
```

**Key questions answered before writing the loop:**

| Question | Answer |
|----------|--------|
| What changes each repetition? | Loan balance |
| What stays the same? | Repayment percentage |
| When does it stop? | When loan balance ≤ 0 |

If you cannot answer these three questions, your loop logic will not work.

---

## Part 6: Looking Ahead — Programming Becomes More Complex

As you progress:

* Problems will combine multiple logical structures
* Decisions may appear inside loops
* Loops may be nested
* Different loop types will be introduced
* Structures will become more layered

This is a natural progression.

The same approach still applies:

* Break the problem down
* Use IPO
* Plan before coding
* Build step by step

---

## Final Reminder

There is no single “correct” way to think.

Your lecturer demonstrates **one structured approach** to help you develop your own thinking.

Your goal is to:

* Understand *what* is happening
* Understand *why* it works
* Build your own problem-solving confidence

If you follow this process consistently, you will become less dependent on external help and more confident in your own ability.

---

**Use this document regularly. Keep it nearby when working.  
It is not just notes — it is your thinking toolkit.**
