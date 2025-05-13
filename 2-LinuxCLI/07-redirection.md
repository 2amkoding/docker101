```plaintext
## Redirection

standard input: keyboard
standard output: monitor

redirection: change the standard input/output

ex1:
    cat file1.txt
        output: Hello World
    
    cat file1.txt > file2.txt
    cat file2.txt
        output: Hello World
    
    cat file1.txt file2.txt > combined.txt

ex2:
    echo hello
        output: hello
   
    echo hello > hello.txt
    cat hello.txt
        output: hello

the point: great for adding 1 liners instead of 'nano'


```