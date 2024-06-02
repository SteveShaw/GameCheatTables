## Related Code

```asm
C7 44 24 10 00000000           mov [rsp+10], 00000000
33 C2                          xor eax, edx
2B C2 			       sub eax, edx
48 8D 54 24 10                 lea rax, [rsp+10]
2B C8                          sub ecx, eax
48 8D 44 24 08                 lea, rax, [rsp+08]
85 C9                          test ecx, ecx
89 4C 24 08                    mov [rsp+08], ecx
48 0F4E C2                     cmovle rax, rdx
8B 00                          mov eax, [rax]
41 89 41 58                    mov [r9+58], eax
```
