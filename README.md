# Files-Comparator  
**This project compares between 2 given files.**    
We get 2 files as an arguments to main, and we check either the files are **identical/similar or different**.  
- **Identical** files contains the same content - char to char.  
- **Similar** files are files that contains the same content, but not identical. i.e there is a difference in the use of the chars, such as different use of capital and small letters, spaces and enters (line breaks).  
- **Different** files does not contain the same content (even one letter difference is sufficient).    

For example, the following files are **similar, but not identical:**    
**File A**:  
12ab23  
**File B**:  
12Ab23  
**File C**:  
12aB23  
**File D**:  
12AB23  
**File E**:  
12 aB  23  
**File F**:  
12  
ab2  
3  
  
  
If you wish to run the code, compile it with:  
gcc -o ex21.c comp.out  
Then run the program with 2 files as arguments, for example:  
./comp.out  /home/os2021/code/1.txt  /home/os2021/code/2.txt  

To check either the files are identical/similar or different, write "echo $?". that will give as the returning value from the program.  
The value 1 means that both of the files are identical.   
The value 2 means that the files are different.  
The value 3 means that the files are similar.   
