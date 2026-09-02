Simple Grading System

START

input TE
input Q
input A

Grade = TE * 0.5 + Q * 0.3 + A * 0.2

if Grade > 100 || Grade < 0
    display "No Such Grade Exist"
else if Grade >= 91
    display Grade
    display "A"
else if Grade >= 81
    display Grade
    display "B"
else if Grade >= 71
    display Grade
    display "C"
else if Grade >= 61
    display Grade
    display "D"
else if Grade >= 51
    display Grade
    display "E"
else if Grade > 0
    display Grade
    display "F"
else
    display "No Such Grade Exist"
end

END

              ┌─────────────┐
              │    START    │
              └──────┬──────┘
                     ↓
             ╱───────────────╲
            ╱   Input TE, Q, A ╲
            ╲─────────────────╱
                     ↓
             ┌─────────────────┐
             │ Grade = TE*0.5  │
             │      + Q*0.3    │
             │      + A*0.2    │
             └────────┬────────┘
                      ↓
              ◇────────────────◇
             ╱ Grade > 100 OR   ╲
            ╱     Grade < 0?      ╲
            ◇─────────────────────◇
                ↓ YES       ↓ NO
                ↓             ↓
       ┌────────────────┐    ◇──────────────◇
       │ Display "No    │   ╱  Grade >= 91?  ╲
       │ Such Grade     │   ◇────────────────◇
       │ Exist"         │      ↓ YES    ↓ NO
       └───────┬────────┘      ↓          ↓
               │         ┌──────────┐    ◇──────────────◇
               │         │ Display  │   ╱  Grade >= 81?  ╲
               │         │ Grade, A │   ◇────────────────◇
               │         └────┬─────┘      ↓ YES    ↓ NO
               │              │             ↓          ↓
               │              │       ┌──────────┐    ◇──────────────◇
               │              │       │ Display  │   ╱  Grade >= 71?  ╲
               │              │       │ Grade, B │   ◇────────────────◇
               │              │       └────┬─────┘      ↓ YES    ↓ NO
               │              │            │             ↓          ↓
               │              │            │       ┌──────────┐    ◇──────────────◇
               │              │            │       │ Display  │   ╱  Grade >= 61?  ╲
               │              │            │       │ Grade, C │   ◇────────────────◇
               │              │            │       └────┬─────┘      ↓ YES    ↓ NO
               │              │            │            │             ↓          ↓
               │              │            │            │       ┌──────────┐    ◇──────────────◇
               │              │            │            │       │ Display  │   ╱  Grade >= 51?  ╲
               │              │            │            │       │ Grade, D │   ◇────────────────◇
               │              │            │            │       └────┬─────┘      ↓ YES    ↓ NO
               │              │            │            │            │             ↓          ↓
               │              │            │            │            │       ┌──────────┐    ◇──────────────◇
               │              │            │            │            │       │ Display  │   ╱   Grade > 0?   ╲
               │              │            │            │            │       │ Grade, E │   ◇────────────────◇
               │              │            │            │            │       └────┬─────┘      ↓ YES    ↓ NO
               │              │            │            │            │            │             ↓          ↓
               │              │            │            │            │            │       ┌──────────┐ ┌───────────────┐
               │              │            │            │            │            │       │ Display  │ │ Display "No   │
               │              │            │            │            │            │       │ Grade, F │ │ Such Grade    │
               │              │            │            │            │            │       └────┬─────┘ │ Exist"        │
               │              │            │            │            │            │            │       └──────┬────────┘
               └──────────────┴────────────┴────────────┴────────────┴────────────┴────────────┴──────────────┘
                                                   ↓
                                             ┌───────────┐
                                             │    END    │
                                             └───────────┘














Division Using Repeated Subtraction

START

input Dividend
input Divisor

Quotient = 0
Remainder = Dividend

while Remainder >= Divisor
    Remainder = Remainder - Divisor
    Quotient = Quotient + 1
end

display Quotient
display Remainder

END

             ┌─────────────┐
             │    START    │
             └──────┬──────┘
                    ↓
            ╱─────────────────╲
           ╱ Input Dividend,    ╲
           ╲      Divisor       ╱
            ╲─────────────────╱
                    ↓
            ┌──────────────────┐
            │ Quotient = 0     │
            │ Remainder=Dividend│
            └────────┬─────────┘
                     ↓
              ◇────────────────◇
             ╱ Remainder >=     ╲
            ╱     Divisor?        ╲
            ◇─────────────────────◇
                ↓ YES       ↓ NO
                ↓             ↓
       ┌─────────────────┐  ┌──────────────────┐
       │ Remainder =     │  │ Display Quotient │
       │ Remainder -     │  │ Display Remainder│
       │ Divisor         │  └────────┬─────────┘
       └────────┬────────┘           ↓
                ↓              ┌─────────────┐
       ┌─────────────────┐     │     END     │
       │ Quotient =      │     └─────────────┘
       │ Quotient + 1    │
       └────────┬────────┘
                │
                └───────────────┐
                                ↓
                       ◇ Remainder >=
                         Divisor? ◇


















Cumulative Sum of N Numbers

START

input N
Sum = 0
Count = 1

while Count <= N
    input Number
    Sum = Sum + Number
    Count = Count + 1
end

display Sum

END

                    ╭──────────────╮
                    │    TERMINAL  │
                    │    START     │
                    ╰──────┬───────╯
                           ↓
                 ╱──────────────────╲
                ╱     MANUAL INPUT   ╲
               ╱       Input N        ╲
               ╲──────────────────────╱
                           ↓
                 ┌──────────────────┐
                 │    PREPARATION   │
                 │    Sum = 0       │
                 │    Count = 1     │
                 └────────┬─────────┘
                          ↓
                    ◇─────────────◇
                   ╱ Count <= N ?  ╲
                  ◇─────────────────◇
                    ↓ YES      ↓ NO
                    ↓            ↓
          ╱────────────────╲   ╱──────────────╲
         ╱    MANUAL INPUT  ╲ ╱    DISPLAY     ╲
        ╱     Input Number    ╲    Display Sum   ╲
        ╲────────────────────╱ ╲────────────────╱
                    ↓                  ↓
          ┌──────────────────┐   ╭──────────────╮
          │     PROCESS      │   │   TERMINAL   │
          │ Sum = Sum +      │   │     END      │
          │ Number           │   ╰──────────────╯
          └────────┬─────────┘
                   ↓
          ┌──────────────────┐
          │     PROCESS      │
          │ Count = Count+1  │
          └────────┬─────────┘
                   │
                   └──────────────→ ◇ Count <= N? ◇
















Factor of 3 or 5

START

input N

if N % 3 == 0 || N % 5 == 0
    display "KORIK"
else
    display "EKIS"
end

END


                 ╭──────────────╮
                 │   TERMINAL   │
                 │    START     │
                 ╰──────┬───────╯
                        ↓
               ╱─────────────────╲
              ╱    MANUAL INPUT   ╲
             ╱       Input N        ╲
             ╲─────────────────────╱
                        ↓
                ◇─────────────────◇
               ╱ N % 3 == 0 OR     ╲
              ╱ N % 5 == 0 ?         ╲
              ◇─────────────────────◇
                 ↓ YES         ↓ NO
                 ↓               ↓
       ╱────────────────╲   ╱────────────────╲
      ╱     DISPLAY      ╲ ╱      DISPLAY      ╲
     ╱     "KORIK"        ╲    "EKIS"          ╲
     ╲────────────────────╱ ╲──────────────────╱
                 ↓               ↓
            ╭──────────╮    ╭──────────╮
            │ TERMINAL │    │ TERMINAL │
            │   END    │    │   END    │
            ╰──────────╯    ╰──────────╯













Finding the Minimum in a Range

START

input N
input Number

Minimum = Number
Count = 2

while Count <= N
    input Number

    if Number < Minimum
        Minimum = Number
    end

    Count = Count + 1
end

display Minimum

END

                 ╭──────────────╮
                 │   TERMINAL   │
                 │    START     │
                 ╰──────┬───────╯
                        ↓
               ╱─────────────────╲
              ╱    MANUAL INPUT   ╲
             ╱       Input N        ╲
             ╲─────────────────────╱
                        ↓
               ╱─────────────────╲
              ╱    MANUAL INPUT   ╲
             ╱     Input Number    ╲
             ╲─────────────────────╱
                        ↓
                 ┌──────────────┐
                 │ PREPARATION  │
                 │ Minimum=Num  │
                 │ Count = 2    │
                 └──────┬───────┘
                        ↓
                 ◇─────────────◇
                ╱ Count <= N ?  ╲
               ◇─────────────────◇
                 ↓ YES      ↓ NO
                 ↓            ↓
       ╱────────────────╲     ↓
      ╱   MANUAL INPUT   ╲    ↓
     ╱    Input Number    ╲    ↓
     ╲────────────────────╱    ↓
                ↓              ↓
          ◇──────────────◇     ↓
         ╱ Number <       ╲    ↓
        ╱ Minimum ?         ╲   ↓
        ◇───────────────────◇   ↓
          ↓ YES       ↓ NO     ↓
          ↓             │       ↓
    ┌──────────────┐    │       ↓
    │   PROCESS    │    │       ↓
    │ Minimum =    │    │       ↓
    │ Number       │    │       ↓
    └──────┬───────┘    │       ↓
           └──────┬─────┘       ↓
                  ↓             ↓
          ┌────────────────┐    ↓
          │    PROCESS     │    ↓
          │ Count=Count+1  │    ↓
          └───────┬────────┘    ↓
                  │             ↓
                  └────→ ◇ Count <= N? ◇
                                ↓ NO
                                ↓
                       ╱────────────────╲
                      ╱     DISPLAY      ╲
                     ╱ Display Minimum    ╲
                     ╲────────────────────╱
                                ↓
                         ╭────────────╮
                         │  TERMINAL  │
                         │    END     │
                         ╰────────────╯
















Finding the Maximum in a Range

START

input N
input Number

Maximum = Number
Count = 2

while Count <= N
    input Number

    if Number > Maximum
        Maximum = Number
    end

    Count = Count + 1
end

display Maximum

END











Logarithm of Base 2

START

input N

Log = 0

while N > 1
    N = N / 2
    Log = Log + 1
end

display Log

END

                 ╭──────────────╮
                 │   TERMINAL   │
                 │    START     │
                 ╰──────┬───────╯
                        ↓
               ╱─────────────────╲
              ╱    MANUAL INPUT   ╲
             ╱       Input N        ╲
             ╲─────────────────────╱
                        ↓
                 ┌──────────────┐
                 │ PREPARATION  │
                 │ Log = 0      │
                 └──────┬───────┘
                        ↓
                 ◇─────────────◇
                ╱     N > 1 ?   ╲
               ◇─────────────────◇
                 ↓ YES      ↓ NO
                 ↓            ↓
          ┌──────────────┐     ↓
          │    PROCESS   │     ↓
          │ N = N / 2    │     ↓
          └──────┬───────┘     ↓
                 ↓             ↓
          ┌──────────────┐     ↓
          │    PROCESS   │     ↓
          │ Log = Log+1  │     ↓
          └──────┬───────┘     ↓
                 │             ↓
                 └──────→ ◇ N > 1 ? ◇
                              ↓ NO
                     ╱────────────────╲
                    ╱     DISPLAY      ╲
                   ╱    Display Log     ╲
                   ╲────────────────────╱
                              ↓
                       ╭────────────╮
                       │  TERMINAL  │
                       │    END     │
                       ╰────────────╯



Fibonacci Sequence

START

input N

First = 0
Second = 1
Count = 1

while Count <= N
    display First

    Next = First + Second
    First = Second
    Second = Next

    Count = Count + 1
end

END

                 ╭──────────────╮
                 │   TERMINAL   │
                 │    START     │
                 ╰──────┬───────╯
                        ↓
               ╱─────────────────╲
              ╱    MANUAL INPUT   ╲
             ╱       Input N        ╲
             ╲─────────────────────╱
                        ↓
                 ┌──────────────┐
                 │ PREPARATION  │
                 │ First = 0    │
                 │ Second = 1   │
                 │ Count = 1    │
                 └──────┬───────┘
                        ↓
                 ◇─────────────◇
                ╱ Count <= N ?  ╲
               ◇─────────────────◇
                 ↓ YES      ↓ NO
                 ↓            ↓
             ╱────────────╲    ↓
            ╱   DISPLAY    ╲   ↓
           ╱ Display First  ╲  ↓
           ╲────────────────╱   ↓
                 ↓              ↓
          ┌─────────────────┐   ↓
          │    PROCESS      │   ↓
          │ Next=First+Second│  ↓
          └────────┬────────┘   ↓
                   ↓            ↓
          ┌─────────────────┐   ↓
          │    PROCESS      │   ↓
          │ First = Second   │   ↓
          │ Second = Next    │   ↓
          └────────┬────────┘   ↓
                   ↓            ↓
          ┌─────────────────┐   ↓
          │    PROCESS      │   ↓
          │ Count=Count+1   │   ↓
          └────────┬────────┘   ↓
                   │            ↓
                   └────→ ◇ Count <= N? ◇
                                ↓ NO
                               END
















Percentage of Marks

START

input MarksScored
input TotalMarks

Percentage = MarksScored / TotalMarks * 100

display Percentage

END

             ╭──────────────╮
             │   TERMINAL   │
             │    START     │
             ╰──────┬───────╯
                    ↓
          ╱────────────────────╲
         ╱     MANUAL INPUT     ╲
        ╱ Marks Scored, Total    ╲
        ╲        Marks           ╱
         ╲──────────────────────╱
                    ↓
          ┌────────────────────┐
          │      PROCESS       │
          │ Percentage =       │
          │ MarksScored /      │
          │ TotalMarks * 100   │
          └─────────┬──────────┘
                    ↓
           ╱────────────────╲
          ╱      DISPLAY     ╲
         ╱ Display Percentage ╲
         ╲────────────────────╱
                    ↓
             ╭────────────╮
             │  TERMINAL  │
             │    END     │
             ╰────────────╯











Finding the Factors of a Number

START

input N

Number = 1

while Number <= N
    if N % Number == 0
        display Number
    end

    Number = Number + 1
end

END


             ╭──────────────╮
             │   TERMINAL   │
             │    START     │
             ╰──────┬───────╯
                    ↓
          ╱────────────────────╲
         ╱     MANUAL INPUT     ╲
        ╱ Marks Scored, Total    ╲
        ╲        Marks           ╱
         ╲──────────────────────╱
                    ↓
          ┌────────────────────┐
          │      PROCESS       │
          │ Percentage =       │
          │ MarksScored /      │
          │ TotalMarks * 100   │
          └─────────┬──────────┘
                    ↓
           ╱────────────────╲
          ╱      DISPLAY     ╲
         ╱ Display Percentage ╲
         ╲────────────────────╱
                    ↓
             ╭────────────╮
             │  TERMINAL  │
             │    END     │
             ╰────────────╯












Simple Interest Calculator

START

input P
input R
input T

SI = (P * R * T) / 100

display SI

END 

          ╭──────────────╮
          │   TERMINAL   │
          │    START     │
          ╰──────┬───────╯
                 ↓
        ╱────────────────╲
       ╱    MANUAL INPUT   ╲
      ╱     Input P,R,T     ╲
      ╲──────────────────────╱
                 ↓
        ┌──────────────────┐
        │     PROCESS      │
        │ SI=(P*R*T)/100   │
        └────────┬─────────┘
                 ↓
        ╱────────────────╲
       ╱     DISPLAY       ╲
      ╱    Display SI       ╲
      ╲────────────────────╱
                 ↓
          ╭────────────╮
          │  TERMINAL  │
          │    END     │
          ╰────────────╯
















Cumulative Sum of Even Numbers up to N

START

input N

Sum = 0
Number = 2

while Number <= N
    Sum = Sum + Number
    Number = Number + 2
end

display Sum

END


                 ╭──────────────╮
                 │   TERMINAL   │
                 │    START     │
                 ╰──────┬───────╯
                        ↓
              ╱──────────────────╲
             ╱    MANUAL INPUT    ╲
            ╱       Input N        ╲
            ╲──────────────────────╱
                        ↓
              ┌──────────────────┐
              │    PREPARATION   │
              │    Sum = 0       │
              │    Number = 2    │
              └────────┬─────────┘
                       ↓
                 ◇──────────────◇
                ╱ Number <= N ?  ╲
               ◇──────────────────◇
                 ↓ YES       ↓ NO
                 ↓             ↓
          ┌──────────────┐      ↓
          │    PROCESS   │      ↓
          │ Sum=Sum+     │      ↓
          │ Number       │      ↓
          └──────┬───────┘      ↓
                 ↓              ↓
          ┌──────────────┐      ↓
          │    PROCESS   │      ↓
          │ Number=      │      ↓
          │ Number + 2   │      ↓
          └──────┬───────┘      ↓
                 │              ↓
                 └──────→ ◇ Number <= N? ◇
                                ↓ NO
                       ╱────────────────╲
                      ╱     DISPLAY      ╲
                     ╱    Display Sum     ╲
                     ╲────────────────────╱
                                ↓
                         ╭────────────╮
                         │  TERMINAL  │
                         │    END     │
                         ╰────────────╯










Collatz Conjecture

START

input N

while N != 1

    display N

    if N % 2 == 0
        N = N / 2
    else
        N = N * 3 + 1
    end

end

display N

END

                 ╭──────────────╮
                 │   TERMINAL   │
                 │    START     │
                 ╰──────┬───────╯
                        ↓
              ╱──────────────────╲
             ╱    MANUAL INPUT    ╲
            ╱       Input N        ╲
            ╲──────────────────────╱
                        ↓
                 ◇─────────────◇
                ╱    N != 1 ?   ╲
               ◇─────────────────◇
                 ↓ YES      ↓ NO
                 ↓            ↓
          ╱──────────────╲     ↓
         ╱     DISPLAY    ╲    ↓
        ╱    Display N     ╲    ↓
        ╲──────────────────╱    ↓
                 ↓              ↓
          ◇────────────────◇    ↓
         ╱   N % 2 == 0 ?   ╲   ↓
        ◇────────────────────◇  ↓
          ↓ YES        ↓ NO     ↓
          ↓              ↓      ↓
    ┌──────────────┐ ┌───────────────┐
    │    PROCESS   │ │    PROCESS    │
    │ N = N / 2    │ │ N = N * 3 + 1 │
    └──────┬───────┘ └───────┬───────┘
           │                  │
           └────────┬─────────┘
                    ↓
               ◇ N != 1 ? ◇
                    ↓ NO
             ╱──────────────╲
            ╱     DISPLAY    ╲
           ╱    Display N     ╲
           ╲──────────────────╱
                    ↓
             ╭────────────╮
             │  TERMINAL  │
             │    END     │
             ╰────────────╯










Sum of Multiples of 3

START

Sum = 0

input Number

while Number >= 0

    if Number % 3 == 0
        Sum = Sum + Number
    end

    input Number
end

display Sum

END

                 ╭──────────────╮
                 │   TERMINAL   │
                 │    START     │
                 ╰──────┬───────╯
                        ↓
                 ┌──────────────┐
                 │ PREPARATION  │
                 │    Sum = 0   │
                 └──────┬───────┘
                        ↓
              ╱──────────────────╲
             ╱    MANUAL INPUT    ╲
            ╱    Input Number      ╲
            ╲──────────────────────╱
                        ↓
                 ◇───────────────◇
                ╱  Number >= 0 ?  ╲
               ◇───────────────────◇
                 ↓ YES       ↓ NO
                 ↓             ↓
          ◇────────────────◇   ↓
         ╱ Number % 3 == 0? ╲  ↓
        ◇────────────────────◇ ↓
          ↓ YES       ↓ NO     ↓
          ↓             │       ↓
    ┌──────────────┐    │       ↓
    │    PROCESS   │    │       ↓
    │ Sum=Sum+     │    │       ↓
    │ Number       │    │       ↓
    └──────┬───────┘    │       ↓
           └──────┬─────┘       ↓
                  ↓             ↓
          ╱──────────────────╲  ↓
         ╱    MANUAL INPUT    ╲ ↓
        ╱    Input Number      ╲ ↓
        ╲──────────────────────╱ ↓
                  │              ↓
                  └────→ ◇ Number >= 0? ◇
                                  ↓ NO
                         ╱────────────────╲
                        ╱     DISPLAY      ╲
                       ╱    Display Sum     ╲
                       ╲────────────────────╱
                                  ↓
                           ╭────────────╮
                           │  TERMINAL  │
                           │    END     │
                           ╰────────────╯









Which Number Has More Factors

START

input Number1
input Number2

Count1 = 0
Count2 = 0
Number = 1

while Number <= Number1
    if Number1 % Number == 0
        Count1 = Count1 + 1
    end
    Number = Number + 1
end

Number = 1

while Number <= Number2
    if Number2 % Number == 0
        Count2 = Count2 + 1
    end
    Number = Number + 1
end

if Count1 > Count2
    display Number1, "has more factors"
else if Count2 > Count1
    display Number2, "has more factors"
else
    display "They have equal factors"
end

END


                    ╭──────────────╮
                    │   TERMINAL   │
                    │    START     │
                    ╰──────┬───────╯
                           ↓
                 ╱──────────────────╲
                ╱    MANUAL INPUT    ╲
               ╱ Input Number1, Number2 ╲
               ╲────────────────────────╱
                           ↓
                 ┌──────────────────┐
                 │    PREPARATION   │
                 │ Count1 = 0       │
                 │ Number = 1       │
                 └────────┬─────────┘
                          ↓
                  ◇────────────────◇
                 ╱ Number <= Number1 ╲
                ◇──────────────────────◇
                  ↓ YES         ↓ NO
                  ↓               ↓
           ◇────────────────◇     ↓
          ╱ Number1 % Number ╲    ↓
         ╱      == 0 ?         ╲   ↓
         ◇──────────────────────◇  ↓
           ↓ YES       ↓ NO       ↓
           ↓             │         ↓
    ┌──────────────┐     │         ↓
    │    PROCESS   │     │         ↓
    │ Count1=      │     │         ↓
    │ Count1 + 1   │     │         ↓
    └──────┬───────┘     │         ↓
           └──────┬──────┘         ↓
                  ↓                ↓
          ┌────────────────┐       ↓
          │    PROCESS     │       ↓
          │ Number=Number+1│       ↓
          └───────┬────────┘       ↓
                  │                ↓
                  └──────→ ◇ Number <= Number1? ◇
                                      ↓ NO
                           ┌──────────────────┐
                           │    PREPARATION   │
                           │ Count2 = 0       │
                           │ Number = 1       │
                           └────────┬─────────┘
                                    ↓
                           ◇ Number <= Number2? ◇
                              ↓ YES       ↓ NO
                              ↓             ↓
                     ◇ Number2 % Number == 0? ◇
                        ↓ YES        ↓ NO
                        ↓              │
                 [Count2=Count2+1]    │
                        └──────┬───────┘
                               ↓
                        [Number=Number+1]
                               │
                               └──→ ◇ Number <= Number2? ◇
                                             ↓ NO
                                    ◇ Count1 > Count2? ◇
                                      ↓ YES      ↓ NO
                                      ↓            ↓
                             ╱────────────╲    ◇ Count2 > Count1? ◇
                            ╱    DISPLAY   ╲      ↓ YES      ↓ NO
                           ╱ Number1 has   ╲      ↓            ↓
                           ╲ more factors  ╱ ╱──────────╲ ╱──────────────╲
                            ╲────────────╱ ╱  DISPLAY   ╲ ╱    DISPLAY    ╲
                                      │   ╱ Number2 has ╲ ╱ They have     ╲
                                      │   ╲ more factors╱ ╲ equal factors ╱
                                      │    ╲───────────╱   ╲──────────────╱
                                      └─────────┬──────────────┘
                                                ↓
                                         ╭────────────╮
                                         │  TERMINAL  │
                                         │    END     │
                                         ╰────────────╯
















Frequency Counter of Numbers

START

input N

Count = 1

while Count <= N
    input Number
    Count = Count + 1
end

display the frequency of each number

END

                 ╭──────────────╮
                 │   TERMINAL   │
                 │    START     │
                 ╰──────┬───────╯
                        ↓
              ╱──────────────────╲
             ╱    MANUAL INPUT    ╲
            ╱       Input N        ╲
            ╲──────────────────────╱
                        ↓
                 ┌──────────────┐
                 │ PREPARATION  │
                 │ Count = 1    │
                 └──────┬───────┘
                        ↓
                 ◇ Count <= N? ◇
                   ↓ YES   ↓ NO
                   ↓         ↓
          ╱──────────────╲    ↓
         ╱  MANUAL INPUT  ╲   ↓
        ╱   Input Number   ╲  ↓
        ╲──────────────────╱  ↓
                   ↓           ↓
          ┌────────────────┐  ↓
          │     PROCESS    │  ↓
          │  Store Number  │  ↓
          └───────┬────────┘  ↓
                  ↓            ↓
          ┌────────────────┐  ↓
          │    PROCESS     │  ↓
          │ Count=Count+1  │  ↓
          └───────┬────────┘  ↓
                  │            ↓
                  └──→ ◇ Count <= N? ◇
                              ↓ NO
                   ┌────────────────────┐
                   │     PROCESS        │
                   │ Select next unique │
                   │ Number             │
                   └─────────┬──────────┘
                             ↓
                     ┌────────────────┐
                     │   PREPARATION  │
                     │ Frequency = 0  │
                     └───────┬────────┘
                             ↓
                    ◇ More stored numbers? ◇
                       ↓ YES         ↓ NO
                       ↓               ↓
             ◇ Stored Number ==        │
               Unique Number? ◇        │
                ↓ YES    ↓ NO          │
                ↓          │            │
          [Frequency=      │            │
           Frequency+1]    │            │
                └────┬─────┘            │
                     ↓                  │
                    next ───────────────┘
                                         ↓
                              ╱──────────────────╲
                             ╱      DISPLAY      ╲
                            ╱ Unique Number and   ╲
                            ╲     Frequency       ╱
                             ╲────────────────────╱
                                         ↓
                                More unique numbers?
                                  ↓ YES       ↓ NO
                                  └──→ back    ↓
                                             END














Factorial of a Number

START

input N

Factorial = 1
Number = 1

while Number <= N
    Factorial = Factorial * Number
    Number = Number + 1
end

display Factorial

END

                 ╭──────────────╮
                 │   TERMINAL   │
                 │    START     │
                 ╰──────┬───────╯
                        ↓
              ╱──────────────────╲
             ╱    MANUAL INPUT    ╲
            ╱       Input N        ╲
            ╲──────────────────────╱
                        ↓
                 ┌──────────────┐
                 │ PREPARATION  │
                 │ Factorial=1  │
                 │ Number=1     │
                 └──────┬───────┘
                        ↓
                 ◇ Number <= N? ◇
                   ↓ YES    ↓ NO
                   ↓          ↓
             ┌──────────────┐  ↓
             │    PROCESS   │  ↓
             │ Factorial =  │  ↓
             │ Factorial *  │  ↓
             │ Number       │  ↓
             └──────┬───────┘  ↓
                    ↓           ↓
             ┌──────────────┐  ↓
             │    PROCESS   │  ↓
             │ Number=      │  ↓
             │ Number + 1   │  ↓
             └──────┬───────┘  ↓
                    │           ↓
                    └──→ ◇ Number <= N? ◇
                                      ↓ NO
                            ╱────────────────╲
                           ╱     DISPLAY      ╲
                          ╱ Display Factorial  ╲
                          ╲────────────────────╱
                                      ↓
                               ╭────────────╮
                               │  TERMINAL  │
                               │    END     │
                               ╰────────────╯

















Area and Perimeter of Basic Shapes

START

display "1. Rectangle"
display "2. Triangle"
display "3. Circle"

input Choice

if Choice == 1

    input L
    input W

    Area = L * W
    Perimeter = 2 * (L + W)

    display Area
    display Perimeter

else if Choice == 2

    input B
    input H

    Area = 0.5 * B * H

    display Area

else if Choice == 3

    input R

    Area = 3.14159 * R * R
    Circumference = 2 * 3.14159 * R

    display Area
    display Circumference

end

END


                     ╭──────────────╮
                     │   TERMINAL   │
                     │    START     │
                     ╰──────┬───────╯
                            ↓
                   ╱────────────────╲
                  ╱      DISPLAY     ╲
                 ╱ 1. Rectangle      ╲
                 ╲ 2. Triangle       ╱
                  ╲ 3. Circle       ╱
                   ╲────────────────╱
                            ↓
                  ╱──────────────────╲
                 ╱    MANUAL INPUT    ╲
                ╱      Input Choice    ╲
                ╲──────────────────────╱
                            ↓
                    ◇ Choice == 1? ◇
                     ↓ YES      ↓ NO
                     ↓            ↓
             ╱──────────────╲      ↓
            ╱  MANUAL INPUT  ╲     ↓
           ╱     Input L,W    ╲     ↓
           ╲──────────────────╱     ↓
                     ↓              ↓
             ┌──────────────┐      ↓
             │    PROCESS   │      ↓
             │ Area=L*W     │      ↓
             └──────┬───────┘      ↓
                    ↓              ↓
             ┌──────────────┐      ↓
             │    PROCESS   │      ↓
             │ P=2*(L+W)    │      ↓
             └──────┬───────┘      ↓
                    ↓              ↓
             ╱──────────────╲      ↓
            ╱    DISPLAY     ╲     ↓
           ╱ Area, Perimeter  ╲    ↓
           ╲──────────────────╱     ↓
                    ↓              ↓
                   END             ↓

                              ◇ Choice == 2? ◇
                               ↓ YES      ↓ NO
                               ↓            ↓
                       ╱──────────────╲     ↓
                      ╱  MANUAL INPUT  ╲    ↓
                     ╱     Input B,H    ╲    ↓
                     ╲──────────────────╱    ↓
                               ↓             ↓
                       ┌──────────────┐      ↓
                       │    PROCESS   │      ↓
                       │ A=0.5*B*H    │      ↓
                       └──────┬───────┘      ↓
                              ↓               ↓
                       ╱──────────────╲       ↓
                      ╱    DISPLAY     ╲      ↓
                     ╱      Area       ╲      ↓
                     ╲──────────────────╱      ↓
                              ↓               ↓
                             END              ↓

                                      ◇ Choice == 3? ◇
                                       ↓ YES      ↓ NO
                                       ↓            ↓
                               ╱──────────────╲    ↓
                              ╱  MANUAL INPUT  ╲   ↓
                             ╱     Input R      ╲  ↓
                             ╲──────────────────╱   ↓
                                       ↓            ↓
                               ┌──────────────┐     ↓
                               │    PROCESS   │     ↓
                               │ A=π*R*R      │     ↓
                               └──────┬───────┘     ↓
                                      ↓             ↓
                               ┌──────────────┐     ↓
                               │    PROCESS   │     ↓
                               │ C=2*π*R      │     ↓
                               └──────┬───────┘     ↓
                                      ↓             ↓
                               ╱──────────────╲     ↓
                              ╱    DISPLAY     ╲    ↓
                             ╱ Area, Circumference ╲
                             ╲──────────────────────╱
                                      ↓             ↓
                                     END ←──────────┘


















Area of a Regular Polygon

START

input N
input Side
input Apothem

Perimeter = N * Side
Area = 0.5 * Perimeter * Apothem

display Area

END
                 ╭──────────────╮
                 │   TERMINAL   │
                 │    START     │
                 ╰──────┬───────╯
                        ↓
              ╱──────────────────╲
             ╱    MANUAL INPUT    ╲
            ╱ Input N, Side,       ╲
            ╲     Apothem          ╱
             ╲─────────────────────╱
                        ↓
                 ┌──────────────┐
                 │    PROCESS   │
                 │ Perimeter =  │
                 │ N * Side     │
                 └──────┬───────┘
                        ↓
                 ┌──────────────┐
                 │    PROCESS   │
                 │ Area = 0.5 * │
                 │ Perimeter *   │
                 │ Apothem       │
                 └──────┬───────┘
                        ↓
                ╱────────────────╲
               ╱     DISPLAY      ╲
              ╱    Display Area    ╲
              ╲────────────────────╱
                        ↓
                 ╭────────────╮
                 │  TERMINAL  │
                 │    END     │
                 ╰────────────╯



















Finding Prime Factors

START

input N

Factor = 2

while N > 1

    if N % Factor == 0
        display Factor
        N = N / Factor
    else
        Factor = Factor + 1
    end

end

END

                 ╭──────────────╮
                 │   TERMINAL   │
                 │    START     │
                 ╰──────┬───────╯
                        ↓
              ╱──────────────────╲
             ╱    MANUAL INPUT    ╲
            ╱       Input N        ╲
            ╲──────────────────────╱
                        ↓
                 ┌──────────────┐
                 │ PREPARATION  │
                 │ Factor = 2   │
                 └──────┬───────┘
                        ↓
                   ◇ N > 1? ◇
                    ↓ YES ↓ NO
                    ↓       ↓
             ◇ N % Factor == 0? ◇
               ↓ YES       ↓ NO
               ↓             ↓
       ╱──────────────╲   ┌──────────────┐
      ╱    DISPLAY     ╲  │    PROCESS   │
     ╱ Display Factor   ╲ │ Factor=      │
     ╲──────────────────╱ │ Factor + 1   │
              ↓            └──────┬───────┘
       ┌──────────────┐           │
       │    PROCESS   │           │
       │ N = N /      │           │
       │ Factor       │           │
       └──────┬───────┘           │
              │                   │
              └─────────┬─────────┘
                        ↓
                    ◇ N > 1? ◇
                       ↓ NO
                      END




















Range Minimum and Maximum

START

input N
input Number

Minimum = Number
Maximum = Number
Count = 2

while Count <= N

    input Number

    if Number < Minimum
        Minimum = Number
    end

    if Number > Maximum
        Maximum = Number
    end

    Count = Count + 1

end

display Minimum
display Maximum

END



                    ╭──────────────╮
                    │   TERMINAL   │
                    │    START     │
                    ╰──────┬───────╯
                           ↓
                 ╱──────────────────╲
                ╱    MANUAL INPUT    ╲
               ╱       Input N        ╲
               ╲──────────────────────╱
                           ↓
                 ╱──────────────────╲
                ╱    MANUAL INPUT    ╲
               ╱     Input Number     ╲
               ╲──────────────────────╱
                           ↓
                 ┌──────────────────┐
                 │    PREPARATION   │
                 │ Minimum = Number │
                 │ Maximum = Number │
                 │ Count = 2        │
                 └────────┬─────────┘
                          ↓
                   ◇ Count <= N? ◇
                    ↓ YES    ↓ NO
                    ↓          ↓
           ╱────────────────╲  ↓
          ╱   MANUAL INPUT   ╲ ↓
         ╱    Input Number    ╲ ↓
         ╲────────────────────╱ ↓
                    ↓           ↓
             ◇ Number < Minimum? ◇
               ↓ YES       ↓ NO
               ↓             │
       ┌────────────────┐     │
       │    PROCESS     │     │
       │ Minimum=Number │     │
       └───────┬────────┘     │
               └──────┬───────┘
                      ↓
             ◇ Number > Maximum? ◇
               ↓ YES       ↓ NO
               ↓             │
       ┌────────────────┐     │
       │    PROCESS     │     │
       │ Maximum=Number │     │
       └───────┬────────┘     │
               └──────┬───────┘
                      ↓
              ┌────────────────┐
              │    PROCESS     │
              │ Count=Count+1  │
              └───────┬────────┘
                      │
                      └────→ ◇ Count <= N? ◇
                                      ↓ NO
                            ╱────────────────╲
                           ╱     DISPLAY      ╲
                          ╱   Display Minimum  ╲
                          ╲────────────────────╱
                                      ↓
                            ╱────────────────╲
                           ╱     DISPLAY      ╲
                          ╱   Display Maximum  ╲
                          ╲────────────────────╱
                                      ↓
                               ╭────────────╮
                               │  TERMINAL  │
                               │    END     │
                               ╰────────────╯