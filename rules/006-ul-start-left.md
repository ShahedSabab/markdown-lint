---
title: MD006 - Consider starting bulleted lists at the beginning of the line
tags:  [bullet, ul, indentation]
alias: ul-start-left
---

This rule is triggered when top level lists don't start at the beginning of a
line:

    Some text

      * List item
      * List item

To fix, ensure that top level list items are not indented:


    Some test

    * List item
    * List item

Rationale: Starting lists at the beginning of the line means that nested list
items can all be indented by the same amount when an editor's indent function
or the tab key is used to indent. Starting a list 1 space in means that the
indent of the first nested list is less than the indent of the second level (3
characters if you use 4 space tabs, or 1 character if you use 2 space tabs).
