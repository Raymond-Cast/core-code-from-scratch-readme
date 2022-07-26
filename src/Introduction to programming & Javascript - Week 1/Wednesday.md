# Challenges
___

## 1. **Your date of birth in the matrix?**

11110111111001000 

[March 13th, 1992]

___

## 2. **MIPS Exercise**

### 2.1 Create a program that adds any two given numbers provided by the user

```assembly
.data
        number_1: .asciiz "\nEnter your first number: "
        number_2: .asciiz "\nEnter your second number: "
        result: .asciiz "\nThe result is "

.text
    main:
        # first input
        li $v0, 4
        la $a0, n1
        syscall

        li $v0, 5
        syscall

        move $t0, $v0
        
        # second input
        li $v0, 4
        la $a0, n2
        syscall
        
        li $v0, 5
        syscall
        
        move $t1, $v0
        
        # calculate and print the result.     
        add $t2, $t0, $t1

        li $v0, 4
        la $a0, result
        syscall

        li $v0, 1
        move $a0, $t2
        syscall
```

### 2.2 Create a program that displays your name

```assembly
.data
            my_name: .asciiz "\nRaymond Castañeda\n"

.text
        main:
            li $v0, 4
            la $a0, my_name
            syscall
```