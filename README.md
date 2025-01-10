# Elixir Enum.each and throw Behavior

This example demonstrates a subtle issue in Elixir's `Enum.each` when used with a `throw` statement. The `throw` in this context doesn't interrupt execution immediately within the anonymous function, leading to unexpected code execution after the `throw` statement, before the exception is finally raised.