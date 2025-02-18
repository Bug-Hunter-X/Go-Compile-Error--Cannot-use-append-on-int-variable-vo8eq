# Go Compile-Time Error: Invalid use of append

This example demonstrates a common Go compile-time error arising from the misuse of the `append` function. The `append` function is designed to work with slices, not individual integer variables.

The `bug.go` file contains code that attempts to append to an integer variable, resulting in a compilation error. The `bugSolution.go` provides a corrected version.

**How to Reproduce:**
1. Save the code in `bug.go`.
2. Attempt to compile using `go build bug.go`.

**Expected Outcome:**
The code will not compile and you will receive a compile-time error message indicating that append cannot be used with an integer.

**Solution:**
The correct approach involves using slices.  The `bugSolution.go` file shows the proper way to use `append`.