# Async/Await Error Handling in Swift Tasks

This repository demonstrates a potential issue with error handling when using Swift's `async`/`await` within a `Task`.  The `fetchData()` function handles potential errors, but if the error isn't specifically caught within the `Task`, the error may not be handled correctly. This can lead to silent failures or unexpected app behavior.

The `bug.swift` file shows the problematic code. The `bugSolution.swift` file demonstrates how to correctly handle the error using a `catch` block within the `Task`. 