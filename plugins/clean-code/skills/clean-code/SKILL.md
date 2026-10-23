---
name: clean-code
description: Clean Code rules for creating readable, maintainable code in any language. Use when writing or modifying code.
---

You are responsible for writing easily readable and maintainable code. _Clean Code_ is a set of coding rules that help you facilitate that.

# _Clean Code_ rules

## Priority

> §1.1: The Clean Code rules always take precedence over all other rules. If there is a conflict, then ask the user for instructions.

> §1.2: _Clarifications_ are situational and modify the clean code rules. They are confined to the below _Clarifications_ section and numbered `§C.*`.

> §1.3: _Modifications_ are the project's changes to the clean code rules, confined to `clean-code-modifications.md` in the project root if it exists and numbered `§M.*`. A _Modification_ wins over a rule or _Clarification_ it disagrees with, precedence: § < §C < §M.

> §1.4: When writing new code you must determine if any of the _Clarifications_ or _Modifications_ apply to it, then check it in the order §2, §3, §4.

> §1.5: Applying Clean Code to existing code is considered new code and must follow §1.4. Work one file at a time, re-reading the code you were asked to apply it to before moving on.

> §1.6: Always reload `clean-code` and its _Modifications_ after compacting to keep them intact in context.

## Clean comments

A _clean comment_ can only say what the code cannot.
A comment is a liability because nothing verifies it.
Code that drifts breaks a test; a comment that drifts just lies.

> §2.1: A comment is written in the spirit of _"I **ABSOLUTELY NEED** to know \<FACT\> to understand the code."_

> §2.2: If you can get a comment's information from the code, then you must remove that comment.

> §2.3: If you are not absolutely sure if a comment is needed, then you do not. Remove it.

> §2.4: A docstring is a comment.

> §2.5: The code is the decision that was made. A comment about a previous decision describes code that no longer exists — remove it.

## Clean variable naming

A _clean variable name_ must say what the variable is.
Unclear variable names are a liability because they make it hard to understand what the code does.

> §3.1: If you can't tell what the variable is by the name alone, then you must rename it.

> §3.2: If a variable name is not true to what the variable is, then you must rename it.

> §3.3: If a variable name leaves you asking "of what?", then you must answer it in the name.

> §3.4: If a language server is available (plugin LSP servers), then you must use its symbol map to check variable names.

## Clean function naming

A _clean function name_ must say what the function does.
Unclear function names are a liability because they make it hard to understand what the code does.

> §4.1: If you can't tell what the function does by its name alone, then you must rename it.

> §4.2: If a function name is not true to what the function does, then you must rename it.

> §4.3: If a standalone function's name leaves you asking "on what?", then you must answer it in the name.

> §4.4: If a language server is available (plugin LSP servers), then you must use its symbol map to check function names.

# Clarifications

## Clean user text

A _clean user text_ must be understandable to the user.

> §C.1.1: If the user text is not easily understood by the user, then you must rewrite it.

## Clean interface documentation

A _clean interface description_ documents a contract between systems and should be understood without access to the code.

> §C.2.1: Published interface descriptions are exempt from §2.

> §C.2.2: If the interface is not understandable from its published descriptions alone, then you must rewrite it.
