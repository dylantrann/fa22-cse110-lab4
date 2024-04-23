# Part 1
1. `values added: 20`

2. `final result: 20`

3. `values added: 20`

4. Code returns an error. This is because the variable `result` is out of scope when trying to access it. It only exists within the if statement.

5. Code returns an error. The code attempts to change the value of the variable `result`, which isn't possible since it was declared as a `const`. Thus, an error is returned.

6. Code returns an error. This is for the same reason as #5, such that the variable to be printed (i.e. `result`) was tampered with and that wasn't allowed since it had a `const` declaration. 