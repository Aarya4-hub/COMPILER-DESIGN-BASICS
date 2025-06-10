# COMPILER-DESIGN-BASICS

COMPANY NAME -CODTECH IT SOLUTIONS

NAME -AARYA DIPAK POUL

INTERN ID -CT08DK522

DOMAIN NAME -C++ PROGRAMMING

DURATION -8 WEEKS(APRIL 20th to JUNE 20th 2025)

MENTOR -NEELA SANTHOSH KUMAR


📍Overview


The Arithmetic Expression Evaluator is a fundamental project rooted in the concepts of Compiler Design, specifically in areas like lexical analysis, parsing, and evaluation. This project takes an infix arithmetic expression as input (e.g., (3 + 5) * 2) and computes its result following the rules of operator precedence and associativity. The implementation is done using C++, and it employs stacks to manage operators and operands, similar to how expression parsing and evaluation is handled in compilers.

This tool demonstrates how a compiler would process and evaluate arithmetic expressions, making it a practical exercise in simulating the front-end processing of a compiler. The logic mimics part of a compiler's job — from tokenizing and syntax checking to evaluating the resulting abstract syntax tree (in simplified form using stacks).




🛠️How It Works

The evaluator simulates the evaluation phase of an expression compiler by following key stages similar to lexing, parsing, and semantic evaluation:

Initialization:
Two stacks are declared:

One to hold integers (operands).

Another to hold operators.

Input is read as a string from the user.

Lexical Analysis (Tokenization):
The input string is scanned character by character.

Digits are grouped into full numbers (multi-digit support) and pushed to the operand stack.

Operators and parentheses are identified and managed appropriately.

Parsing and Evaluation:
If the character is a digit, it is parsed as a full number.

If the character is an operator, it is pushed to the operator stack after handling precedence.

If a closing parenthesis ) is found, operators are popped and applied until the matching ( is encountered.

At the end, remaining operators are applied to the remaining operands.

Operator Precedence Handling:
Precedence is respected using a while-loop that checks whether the current operator should immediately apply operations before pushing.

Multiplication and division are given higher priority than addition and subtraction.

This is analogous to how a compiler uses a precedence table or parsing algorithm to build an expression tree.

Final Evaluation:
Once all characters are processed, any remaining operations are resolved.

The final value at the top of the operand stack is the result of the expression.



📌Features


Support for Multi-Digit Numbers: Unlike basic calculators, this evaluator parses entire numbers, not just single digits.

Operator Precedence Handling: Accurately mimics how compilers evaluate precedence (*, / over +, -).

Parenthesis Support: Implements correct grouping and nested expression evaluation.

Division-by-Zero Detection: Prevents undefined behavior by catching and throwing runtime errors.

Error Handling: Uses C++ exception handling to manage invalid expressions like divide-by-zero.

Stack-Based Architecture: Closely simulates a compiler’s use of data structures during evaluation.



📚Learning Objectives


This project helps reinforce essential compiler design concepts and programming skills:

Lexical Analysis:
Recognize and tokenize numeric literals and operators.

Handle whitespace and input formatting, similar to a real lexer.

Parsing Techniques:
Learn how to simulate parsing using stacks.

Understand how infix expressions are parsed and evaluated using precedence rules.

Semantic Evaluation:
Understand how to compute values from expressions — the final stage of front-end compilation.

Reinforces concepts of associativity and operator priority in expression trees.

Error Handling in Compilation:
Introduce basic runtime error checking (e.g., division by zero).

Mimics compiler error handling and diagnostics.

Use of Data Structures:
Apply stacks effectively, mirroring the internal architecture of expression evaluation in real compilers.

Expression Tree Logic (Implied):
Though not building an actual AST (Abstract Syntax Tree), the algorithm follows the same logic in evaluating expressions left-to-right with precedence control.

Hands-On with Operator Algorithms:
Learn algorithmic implementation of mathematical logic often embedded in parsing engines.

Output

![Image](https://github.com/user-attachments/assets/1fa144ee-975a-4d50-a24b-a51cbd63b210)

