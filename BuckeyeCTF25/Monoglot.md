Chimera for multiple architectures
1.  lea rsi, [rip + str]       ; rsi -> address of "Battelle"
    mov edi, 38085             ; rdi = 38085   (arg1)
    mov eax, 237               ; rax = 237     (syscall number)
    syscall
str:
    .ascii "Battelle\0"

2. Thus the hex command would be 488d350c000000bfc5940000b8ed0000000f0542617474656c6c6500.
3. Thus the flag is bctf{a_good_start_4fc9c43c0d95}
