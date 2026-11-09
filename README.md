Work in progress

Currently supports arithmetic expressions

For the test file "test.e" with input ```69 - 2 * 3 * 4 - 2;```
creates output
```asm
mov eax, 69
mov ebx, 2
mov ecx, 3
imul ebx, ecx
mov ecx, 4
imul ebx, ecx
sub eax, ebx
mov ebx, 2
sub eax, ebx
```
