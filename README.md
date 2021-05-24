# VS-debugging-error-record-
Error flag  :
   Run-Time Check Failure #2 - Stack around the variable 'data_error' was corrupted.
Analysis  :
    Run-Time Check Failure #2: 
        Generally, the stack is destroyed, and your code may have problems such as buffer overflow. This problem is caused by memory access errors of some variables, 
        and the error dialog box clearly indicates which variable access is wrong, you can check this variable to get the result. 
    Typical errors: 
        such as defining an array data_error[127]; finally using data_error[127] in your use, or even data_error[128], etc., will cause this error.
