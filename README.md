mips-gcd
========

Finds the GCD of two positive integers using MIPS. Minified as far as I could.

    li $2,5
    syscall
    move $9,$2
    li $2,5
    syscall
    a:bge $9,$2,c
    move $8,$2
    move $2,$9
    move $9,$8
    c:sub $9,$9,$2
    beqz $2,d
    b a
    d:li $2,1
    move $4,$9
    syscall
