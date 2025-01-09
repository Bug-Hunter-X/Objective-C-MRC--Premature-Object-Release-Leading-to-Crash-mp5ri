# Objective-C Manual Reference Counting (MRC) Bug: Premature Release

This repository demonstrates a common yet subtle bug in Objective-C's manual reference counting (MRC) system.  The bug involves the premature release of an object, leading to crashes and unpredictable behavior.

## The Bug
The `bug.m` file contains code that incorrectly releases a string object before its ownership is properly transferred. This leads to a dangling pointer and potential crashes.

## The Solution
The `bugSolution.m` file demonstrates the correct way to manage object lifetimes using `retain`, `release`, and `autorelease` to prevent this memory management error.  Modern Objective-C uses Automatic Reference Counting (ARC), which largely obviates this issue. However, understanding this bug is crucial for comprehending memory management fundamentals and working with legacy code.