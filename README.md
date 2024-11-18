# Assignment 2: Classify

TODO: Add your own descriptions here.


    beq  t0, zero, if_zero_0
    beq  t1, zero, if_zero_0

    blt  zero, t1, start_0
    xori t1, t1, -1
    addi t1, t1, 1
    sub  t0, zero, t0
start_0:
    mv   t2, zero
mul_0:
    andi t3, t1, 1
    beq  t3, zero, conti_0
    add  t2, t2, t0
conti_0:
    srli t1, t1, 1
    slli t0, t0, 1
    bne  t1, zero, mul_0
    j    done_0

if_zero_0:
    mv   t2, zero

done_0:
    mv   a0, t2

###################


    beq  t0, zero, if_zero_1
    beq  t1, zero, if_zero_1

    blt  zero, t1, start_1
    xori t1, t1, -1
    addi t1, t1, 1
    sub  t0, zero, t0
start_1:
    mv   t2, zero
mul_1:
    andi t3, t1, 1
    beq  t3, zero, conti_1
    add  t2, t2, t0
conti_1:
    srli t1, t1, 1
    slli t0, t0, 1
    bne  t1, zero, mul_1
    j    done_1

if_zero_1:
    mv   t2, zero

done_1:
    mv   a1, t2

###################

    beq  t0, zero, if_zero_2
    beq  t1, zero, if_zero_2

    blt  zero, t1, start_2
    xori t1, t1, -1
    addi t1, t1, 1
    sub  t0, zero, t0
start_2:
    mv   t2, zero
mul_2:
    andi t3, t1, 1
    beq  t3, zero, conti_2
    add  t2, t2, t0
conti_2:
    srli t1, t1, 1
    slli t0, t0, 1
    bne  t1, zero, mul_2
    j    done_2

if_zero_2:
    mv   t2, zero

done_2:
    mv   a0, t2



###################
beq  t0, zero, if_zero_3
    beq  t1, zero, if_zero_3

    blt  zero, t1, start_3
    xori t1, t1, -1
    addi t1, t1, 1
    sub  t0, zero, t0
start_3:
    mv   t2, zero
mul_3:
    andi t3, t1, 1
    beq  t3, zero, conti_3
    add  t2, t2, t0
conti_3:
    srli t1, t1, 1
    slli t0, t0, 1
    bne  t1, zero, mul_3
    j    done_3

if_zero_3:
    mv   t2, zero

done_3:
    mv   a1, t2

############


mul  a1, t0, t1

    beq  t0, zero, if_zero_0
    beq  t1, zero, if_zero_0

    blt  zero, t1, start_0
    xori t1, t1, -1
    addi t1, t1, 1
    sub  t0, zero, t0
start_0:
    mv   t2, zero
mul_0:
    andi t3, t1, 1
    beq  t3, zero, conti_0
    add  t2, t2, t0
conti_0:
    srli t1, t1, 1
    slli t2, t2, 1
    bne  t1, zero, mul_0
    j    done_0

if_zero_0:
    mv   t2, zero

done_0:
    mv   a0, t2

