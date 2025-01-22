# Elixir Enum.reduce Missing Return Value

This repository demonstrates a common error in Elixir when using `Enum.reduce`.  The anonymous function within `Enum.reduce` is missing an explicit return value, leading to unexpected behaviour.

The `bug.ex` file shows the erroneous code. The `bugSolution.ex` file provides the corrected version.

This bug is subtle because Elixir implicitly returns the last evaluated expression in a function, but the behavior can be unexpected in anonymous functions within `Enum.reduce` if not handled carefully.