# addStack
### Add Context to Trouble JavaScript errors!

[Initial Pass](http://stackoverflow.com/questions/30132372/adding-stack-trace-reference-to-existing-context-less-error-object)

Ideas
==========================
1) Extend the Error object to add an `.addStack()` method.
2) Callback wrapping method, adding a reference if the error is present.
3) Raw method call `addStack(e)`, returning a modified error.
4) Raw method call `addStack(e)`, returning a combined stack trace (which you could then log / report)

Options
==========================
1) Depth: How far back to capture stack from calling method.
2) Filter by `node_modules/`: Auto-remove references to node_modules in added / returned stack trace.