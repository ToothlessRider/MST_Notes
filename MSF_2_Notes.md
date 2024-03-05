#  MSF Notes for MST
> Author : Aaron Augustine


## Theory of Automata :

> The study of abstract machines and the computational problems solved using these machines is called the Theory of Automata.

### Alphabets :
> They are a finite set of symbols. [ Denoted by Σ ]

  

### String :
> They are a finite set of symbols, strung together, from the alphabet.

  

## Transition Diagram :

![](https://lh7-us.googleusercontent.com/jyQ8o-cdlzV7QpbtxZu-PDr5WOrTjKpfSz4tf9cryX2bwSj4gf7nJnkl5XZxaRBGALxjP0AHpvfPefbetz1_G7MjV3sIoQj-zbHUkqUil9zfgasMcFdE4bn2BJTQCq8WmLDpM9gyPNgHmBog-yV6mIQ)

  
  

## Transition Table :

![](https://lh7-us.googleusercontent.com/qWA48m8JmeiD-a4dZwwoUjUIeQSOE34-a_zlJb9XXOluX8405rQr_gAXdKRq6QAszygZ5yT1UwCjXGLw31VpD_60_hYqyZN5qa0u9u4WGcab4iILxrGZdXQUtMpo9_3Ymu9kPWkakES_Mski7Hz4SQo)


  ==DFA does not have more than a singular entry in each cell
  NFA can have multiple entries in each cell==

## Finite Auomata ~FA~
> Used to recognize patterns
> It has two states, i.e. , "Accept State " or  " Reject State "

It is a collection of 5 tuples ( Q, **Σ**, **δ**, q0, F )
1. Q : Finite set of states 
2. Σ : Finite set of input symbols
3. δ : Transition Function 
4. q0 : Initial State
5. F : Final State

# Deterministic Finite Automata ~DFA~
o In DFA, there is only one path for specific input from the current state to the next state.
o DFA does not accept the null move, i.e., the DFA cannot change state without any input character.
o DFA can contain multiple final states. It is used in Lexical Analysis in Compiler.

L1 = Set of all strings that start with '0'
 -  { 0, 00, 01, 000, 010, 011, 0000, ....... }

Reference Link for DFA video : 
> [DFA by Neso Academy](https://www.youtube.com/watch?v=40i4PKpM0cI)

Q. Construct a DFA that accepts sets of all strings over {0,1} of length 2
Ans. 
**Σ** = { 0,1 }
L = { 00, 01, 10, 11 }

```mermaid
graph LR
A((A)) -- 0,1  --> B((B)) -- 0,1 --> C((C)) -- 0, 1 --> D((D)) 
D -- 0,1 --> D

```

> D here is a dead / trap state

# Non-Deterministic Finite Automata ~NFA~


```mermaid
graph LR
A((A)) -- Link text --> B((B)) -- Link text --> C((C))

```


<hr>

## Questions on transition diagrams and tables

Q1. Create the transition function and transition table for the following inputs : 
δ(q~0~,0) = q~0~ 	δ(q~1~,0) = q~1~, q~2~ δ(q~2~,0) = q~1~ 	δ(q~3~,0) = q~2~ 	δ(q~0~,1) = q~1~ 	δ(q~1~,1) = q~2~ 	δ(q~2~,1) = q~3~ 	δ(q~3~,1) = q~2~

Ans. 
### Transition Diagram


```mermaid  
graph LR
A((q0)) -- 1 --> B((q1)) -- 0 --> C((q2)) -- 1 --> D((q3))

A -- 0 --> A
B -- 0 --> B
B -- 1 --> C
C -- 0 --> B
D -- 0 --> C
D -- 1 --> C

```


### Transition Table
State\Input| 0 | 1 |
--|--|--|
q0 | q0 | q1 | 
q1 | q2, q2 | q2 |
q2 | q1 | q3 |
q3 | q2 | q2 |
> This is an example of Non deterministic Automata because of q1 accepting 0 as input and going to q1 and q2
> 
<hr>

Q2.  Create the transition function and transition table for the following inputs : 
δ(q~0~,0) = q~1~ 	δ(q~0~,1) = q~2~ δ(q~1~,0) = q~0~ 	δ(q~1~,1) = q~2~ 	δ(q~2~,1) = q~2~ 	δ(q~2~,1) = q~2~ 

Ans. 
### Transition Diagram


```mermaid
graph LR
A((q0)) -- 0 --> B((q1)) -- 1 --> C((q2))

A -- 1 --> C
B -- 0 --> A
C -- 0,1 --> C

```


### Transition Table
State\Input| 0 | 1 |
--|--|--|
q0 | q1 | q2 | 
q1 | q0 | q2 |
q2 | q2 | q2 |
<hr>
Q3.  Create the transition function and transition table for the following inputs : 
δ(q~0~,0) = q~0~ 	δ(q~0~,1) = q~1~ δ(q~1~,0) = q~2~ 	δ(q~1~,1) = q~1~ 	δ(q~2~,0) = q~2~ 	δ(q~2~,1) = q~2~ 

Ans. 
### Transition Diagram


```mermaid
graph LR
A((q0)) -- 1 --> B((q1)) -- 0 --> C((q2))

A -- 0 --> A
B -- 1 --> B
C -- 0,1 --> C

```


### Transition Table
State\Input| 0 | 1 |
--|--|--|
q0 | q0 | q1 | 
q1 | q2 | q1 |
q2 | q2 | q2 |

<hr>

Q4. Create the transition function and transition table for the following inputs : 
δ(q~0~,0) = q~0~ 	δ(q~0~,1) = q~2~ δ(q~1~,0) = q~0~ 	δ(q~1~,1) = q~2~ 	δ(q~2~,0) = q~2~ 	δ(q~2~,1) = q~2~ 

Ans. 
### Transition Diagram


```mermaid
graph LR
A((q1)) -- 0 --> B((q0)) -- 1 --> C((q2))

B -- 0 --> B
A -- 1 --> C
C -- 0,1 --> C

```


### Transition Table
State\Input| 0 | 1 |
--|--|--|
q0 | q0 | q2 | 
q1 | q0 | q2 |
q2 | q2 | q2 |

