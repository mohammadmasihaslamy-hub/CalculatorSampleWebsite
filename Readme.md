# How a Calculator Operates

This document describes, at a high level, how a typical electronic or software calculator works.

## Overview

A calculator accepts numeric and operator input, processes that input according to mathematical rules, and returns a numeric result. Calculators can be simple (basic arithmetic) or advanced (scientific, financial).

## Core Components

- Input handling: captures button presses or keyboard entry.
- Display: shows the current entry, expression, and results.
- Parser: interprets the sequence of inputs into numbers and operations.
- Evaluation engine: performs the arithmetic or functional computation.
- Memory and state: stores values for multi-step calculations and supports features like memory recall, clear, and chaining operations.

## Basic Operation Flow

1. User inputs digits and operators (e.g., 12 + 7).
2. The input handler builds the current number and/or expression.
3. The parser/tokenizer converts input into structured tokens (numbers, operators, parentheses).
4. The evaluation engine applies operator precedence (and parentheses) to compute the result.
5. The result is formatted and shown on the display.
6. The calculator updates internal state so the user can continue calculations (e.g., pressing = again repeats the last operation).

## Examples of Evaluation Strategies

- Immediate execution: execute each binary operation as soon as the next operator is entered (common in simple calculators).
- Expression parsing: convert the full expression into postfix (RPN) or use a shunting-yard algorithm, then evaluate (common in scientific calculators and software implementations).

## Error Handling and Edge Cases

- Division by zero: typically shows an error message or special value (e.g., "Error" or "Infinity").
- Overflow/underflow: handle numbers beyond representable range with errors or approximations.
- Invalid input: prevent or report malformed expressions.

## Advanced Features

- Scientific functions: trig, logarithms, powers—usually implemented via math libraries.
- Memory functions: M+, M-, MR, MC to store and recall values.
- History and parentheses: allow complex expressions and review of prior calculations.

This summary captures the typical operation of calculators from input to displayed result.
```
