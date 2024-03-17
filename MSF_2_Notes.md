#  MSF Notes for MST
> Author : Aaron Augustine

> Star the gist so that I can get a consensus on how many people are using this resource

## PYQ's

#### Q1 a. What is FA (finite automata)? Write formal definition of finite automata? Draw the finite automata model diagram and explain input tape finite control.

*Ans*. Finite automata (FA), also referred to as finite-state machines, are ideal for recognizing specific patterns within strings of symbols.
They are

**Formal Definition**

A finite automaton is represented by a 5-tuple:

**Q**: A finite set of states.
**∑**: A finite set of input symbols (the alphabet).
**δ**: The transition function, which maps a state and an input symbol to the next state (Q x ∑ → Q).
**q0**: The initial or start state (an element of Q).
**F**: A set of final or accepting states (a subset of Q)

#### Finite Automata Model Diagram

A finite automata diagram is a visual representation of the following:

**States**: Represented as circles.
**Transitions**: Represented as arrows labeled with input symbols. The arrow points from the current state to the next state based on the input.
**Start State**: Marked with a special arrow pointing towards it.
**Accepting States**: Usually marked with double circles.

**![](https://lh7-us.googleusercontent.com/pta7vwt5BrzDpmXdkmvj62Fq-kGpHUSyAnQ8w6_aIbpIl_BuQ2FpjPtSxV3xPZcLr4nsB3ri5Tsu1uOoYiZaMzoJiUazromog77oW2mah5ShptAp0aPWLz9x5UTLsFUpDVvRZbiu5zR5seGtS7gMTsA)**
**Input tape**: It is a linear tape having some number of cells. Each input symbol is placed in each cell.
**Finite control**: The finite control decides the next state on receiving particular input from input tape. The tape reader reads the cells one by one from left to right, and at a time only one input symbol is read.

<hr>

#### Q1 b. Draw the transition diagram (graph) and write Transition table represent the DFA M =(Q, E, d, q<sub>0</sub>, F) i.e. M ={{q<sub>0</sub>, q<sub>1</sub>, q<sub>2</sub>},{0, 1}, d, q<sub>0</sub>, {q2}}  where d is transition function given by 
| | |
|--|--|
|d(q<sub>0</sub>, 0) = q<sub>0</sub>, q<sub>1</sub>|d(q<sub>0</sub>, 1 ) = q<sub>1</sub>|
|d(q<sub>1</sub>, 0) = q<sub>2</sub>|d(q<sub>1</sub>, 1 ) = q<sub>0</sub>|
|d(q<sub>2</sub>, 0) = q<sub>2</sub>|d(q<sub>2</sub>, 1 ) = q<sub>1</sub>, q<sub>2</sub>|

*Ans* 
### Transition Diagram


**![](https://lh7-us.googleusercontent.com/xqcvfK339ET1H6Fu81dmiBXIwY7st9X6NITmzu2DEs5tny9FODTDNbmVczfNenoDM9nrnUPNIOuWEqGro-cI1J6ZGkOnhtAMwf86KoHHMbTMbylVLDDfpSqRA8BQeEMg0kpNiLYnEwd210Q7NYe4ub0)**


### Transition Table
State\Input| 0 | 1 |
--|--|--|
q0 | q0, q1 | q1 | 
q1 | q2| q0 |
q2 | q0 | q1, q2 |

#### Input Tape and Finite Control

__Input Tape__: A conceptual storage mechanism holding the input string to be processed. It's divided into cells, with each cell containing one input symbol.
__Finite Control__: The brain of the FA. It has a read head that:
- Starts at the leftmost symbol of the input tape.
- Reads one symbol at a time.
- Determines the next state based on the current state and the input symbol using the transition function (δ).
- Moves the read head one cell to the right.


<hr>

#### Q2 a. What is abstract algebra? Explain group, ring, and field. Write properties of group, ring. and field.

*Ans*. It is the branch of algebra dealing with the study of algebraic systems or algebraic structures with one or more mathematical operations associated with element from an identifiable pattern, differing from the usual 

#### Group : 
A group is a set / collection of strings along with one operation
* Ex. ( G, . ) or ( G, + )
This also has the following properties
1. Closure : If & b ∈ S then ( a + b ) ∈ S
2. Associativity : a + ( b + c ) = ( a + b ) + c ( grouping under the sign ) 
3. Identity element : a + 0 = a
4. Inverse element : a + ( -a ) = 0

#### Ring : 
Ring is a set or collection equipped with two binary operations 
* Ex. ( G, +, x )
This also has the following properties
1. Closure ( +, x )
2. Associativity ( +, x )
3. Identity element
4. Inverse element
5. Commutativity : a + b = b + a ( switching under the sign )
6. Distributive law : a( b + c ) = ab + ac

#### Field : 
It is a set / collection of objects  equipped with two binary operations : 
> Main difference b/w field and ring is that that the nonzero elements form an abelian group under multiplication

This also has the following properties
1. Closure ( +, x ) 
2.  Associativity ( +, x )
3. Identity element ( +, x )
4. Inverse element ( +, x )
5. Commutativity ( +, x )
6. Distributive law
7. No zero divisors : If a, b ∈ S & ab = 0, then a = 0 or b = 0

<hr>

#### Q2 b. What is CFG context free grammar
#### Given CFG and Generate the string 'aabb' of given grammar CFG = ( V, T, P, S ) CFG = ( {S}{a, b}, P, S )
Production rule:
* S = aSb
* S = ab


#### Given CFG and generate the string 0101010 of given grammar CFG = ( V, T, P, S ) CFG = ( {S}{0, 1}, P, S )
Production rule: 
* s=0s0 
* s =1s1
* s = 0
* s = 1
* s = ∈

#### Given CFG and generate the string 'baab' of given grammarCFG = ( V, T, P, S ) CFG = ( {S}{0, 1}, P, S )
Production rule: 
* S = aS 
* S = bS
* S = a
* S = b


*Ans* : 

#### Context Free Grammar : 
* It is a model to recognize languages
* Aim is to recognize more languages
* It can recognize all regular and some non-regular languages.

It consists of the following : 
* Terminals
* Variables 
* Substitution
* Start Variable

A context-free grammar is the tuple ( V, Σ, P, S), where
- V is a finite set called *variables*,
- Σ is a finite set disjoint from V called *terminals*,
- P ⊆ V x {V U Σ }* is a finite set of production rules, and
- S ∈ V is the *start variable*.


> Part 1

S --> aSb  put S --> ab
--> aabb
Output string : aabb

> Part 2

s-->0s0 put s-->1s1
-->01s10 put s --> 0s0
-->010s010 put s --> 1s1
--> 0101s1010 put s -->∈
-->0101010
Output String : 0101010
>Part 3

S --> bS put S--> aS
--> baS put S --> aS
--> baaS put S --> b
--> baab
Output String : baab


<hr>

#### Q3a. What is derivation tree or parse tree ? Also solve the following
#### Generate the string p*q+r and draw the derivation tree given that production rule is: 
* E=E+E
* E=p/q/r

*Ans* 
**![](https://lh7-us.googleusercontent.com/9urfhj2CZJvRBa28YCE-wx1-HZtS7b7gMk-pVuWikkkUnIDraDn5VoTZLPNrPH7gFGmgihyW9M918UjojS1VzhHfz0Raon91ycOBdnOyoXixlyFPKYVwrdI0-sb3ONhOmGhWcC0ykMWRytkyAKvvyp4)**


#### Generate the string abbbb and draw the derivation tree given that the production rule is: 
* s = aXY
* y = X
* y = ∈
* x = bYb

*Ans* 
**![](https://lh7-us.googleusercontent.com/FXt5QcriZqZg72FdjWuGwUn8Ah3duq6qyN-Kx1WLurKYbIPdqGdpqJSQwLtaiXu3H0J9QnSbmK2ijI81edYA43qMxB7oEoO4kX-2bUEpILNn7pDgKQpETPAptvhIhkIVl4ANI__9oqvaD2ZD4rvcQNY)**


#### Generate the string aabbaa and draw the derivation tree given that the production rule is : 
* S = aAS
* S = a
* A = SbA
* A = SS
* A = ba

*Ans* 
**![](https://lh7-us.googleusercontent.com/gAULndwgSmUeoez9Vaw37FscMQd3PgQfVxSF-Km7wHhXa7Tgs44FTqA03yp1sajftfk1fXLA8Zf0EeNxHuudxPA1yl20l395fPTMbPS61sFgKAdszjTZnSjSoMgXJYOwvJqHAXr5qdYG__r0k4zJRE0)**

<hr>

#### Q3 b. Write difference between DFA (deterministic finite automata) and NFA (nondeterministic Finite automata).

*Ans* 
**![](https://lh7-us.googleusercontent.com/9YnxehlqZDzB4DVEYFxcyrNEP540WELABzhB2BjNUhZr7ScQY7KOSM-MZU4YP7gY44bK4ohdLTA_2UTEDOcmwVOM57oX-umQcxmo-duWkT4dezwyM--f4wfZsi-fhSY4TSOTehz4J5HrmtvPDW7x_ZI)**

<hr>

#### Q4. What is regular expression? Write the 4 rules of regular expresston Kleene closure(+), concatenation(.), union(U) Draw the finite automata of the given regular expression. The Regular Expression is : 
1. Phi
2. e-Epsilon
3. a
4. b
5. ab
6. a + b
7. a * 
8. a+
9. 01
10. 0 + 1 

*Ans*. Regular Expression or RegEx represents a certain set ( collection ) of strings in some algebraic fashion, accepted by FA.

It is the combination of strings and operations, 
*String* : a, b, c, ...... x, y, z, etc 
*Operations* : +, -, /, * 

Types of reg ex are : 
* *Kleene Closure* ( * ) : 
	* a* = {ε, a, aa, aaa,...... }
* *Positive Closure* ( + ) : 
	* a<sup>+</sup> : { a, aa, aaa, ..... }
* *Concatenation* ( . ) : 
	* ab = {ab}
* *Union* ( U ) : 
	* ( a + b ) = { a, b }

1. Φ (Phi ) 
```mermaid
graph LR
	A((q0))
```

2. ε ( Epsilon ) 
```mermaid
graph LR
	A((qn))
```
> Should be a double circled node to signify end of regular expression

3. a 
```mermaid
graph LR
	A((q0))--a--> B((q1))
```

4. b
```mermaid
graph LR
	A((q0))--b--> B((q1))
```

5. ab
```mermaid
graph LR
	A((q0))--a-->B((q1))--b-->c((q2))
```

6. ( a + b )
```mermaid
graph LR
	A((q0))--a-->B((q1))
	A--b-->B
```

7. a*
```mermaid
graph LR
	A((q0))
	A--a-->A
```

8. a+
```mermaid
graph LR
	A((q0))--a-->B((q1))
	B--a-->B
```

9. 01
```mermaid
graph LR
	A((q0))--0-->B((q1))--1-->C((q2))

```

10. 0 + 1
```mermaid
graph LR
	A((q0))--0-->B((q1))
	A--1-->B
```

<hr>

#### Q4 b. at is SVM support vector machine how does ? What are types of SVM? Draw a suitable diagram to show this. WHat is a Hyperlane what is support vector? What is margin. What is GMM [Gaussian mixture model]?

*Ans* 

## Shortnotes - 56 Page pdf 

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

**![](https://lh7-us.googleusercontent.com/72xvNZ41DhxMJcTmNdjzhSsfFjM_6wTKufKXxMglqiFeiPdkZgsAuuGvebqSihahpWts01_YcXzxjWBf89HsLAUhhtrr8copuU_pNBptgRCF-NY15jVN6xam1qH9m9qm2WfnBNLzU2a-m7PYl_RxqMo)**

> D here is a dead / trap state

# Non-Deterministic Finite Automata ~NFA~


**![](https://lh7-us.googleusercontent.com/PEc02rO0aUFs1ydvl2LVJ160_8Xr1Jq_kCBTpLv59KM0KBxwAfBMyLAbiIaSQNX_tMMnKhM57geZdAqB3SFt0xrFHY4uyIGRpdR1DydI78h7xXGgZBTN4T73PGYaBQV_nMBbP6HvJ6xEOf1w41rXICE)**


<hr>

## Questions on transition diagrams and tables

#### Q1. Create the transition function and transition table for the following inputs : 
δ(q~0~,0) = q~0~ 	δ(q~1~,0) = q~1~, q~2~ δ(q~2~,0) = q~1~ 	δ(q~3~,0) = q~2~ 	δ(q~0~,1) = q~1~ 	δ(q~1~,1) = q~2~ 	δ(q~2~,1) = q~3~ 	δ(q~3~,1) = q~2~

Ans. 
### Transition Diagram


**![](https://lh7-us.googleusercontent.com/j7V3v-XvWMQh7QSVQicGI3DIfUxkZqyqsyTdlkeZpdJjLZgZjLDeU01AylWf4uzxTUKjqKqg6UHUFnzAjOE4XPbhmwlAOjsbgnQar0-wL_JRU4DGRJTafaLmJTYvLwQzbqlOu4NFZhda4TsoLZmX-ok)**


### Transition Table
State\Input| 0 | 1 |
--|--|--|
q0 | q0 | q1 | 
q1 | q2, q2 | q2 |
q2 | q1 | q3 |
q3 | q2 | q2 |
> This is an example of Non deterministic Automata because of q1 accepting 0 as input and going to q1 and q2

<hr>

#### Q2.  Create the transition function and transition table for the following inputs : 
δ(q~0~,0) = q~1~ 	δ(q~0~,1) = q~2~ δ(q~1~,0) = q~0~ 	δ(q~1~,1) = q~2~ 	δ(q~2~,1) = q~2~ 	δ(q~2~,1) = q~2~ 

Ans. 
### Transition Diagram


**![](https://lh7-us.googleusercontent.com/Y-d_6VoIc8uneu1BoL-TPfDbjUAVy70YnL89fcNKuvaPOG3kfQ8ur2yFyMpT1WVszJNLLzaF69Wlbj-NydDxeQOQ4suPYseqJyLwDdIpp-OUEOyPq3l5Ai0-njyaG-rfhCRNoF2PdtmtPj4JvS82T68)**


### Transition Table
State\Input| 0 | 1 |
--|--|--|
q0 | q1 | q2 | 
q1 | q0 | q2 |
q2 | q2 | q2 |

<hr>

#### Q3.  Create the transition function and transition table for the following inputs : 
δ(q~0~,0) = q~0~ 	δ(q~0~,1) = q~1~ δ(q~1~,0) = q~2~ 	δ(q~1~,1) = q~1~ 	δ(q~2~,0) = q~2~ 	δ(q~2~,1) = q~2~ 

Ans. 
### Transition Diagram


**![](https://lh7-us.googleusercontent.com/ExAXUoPd0EM0u6woi1APWhZdw4QJWSysMy7pswUbw-tQy3k0X_mml3H9Bd-e4EZgPcV1Tfb035JlNMh4ZcoCZjDWa-dh89ZOksIVB6qz3F1OOq-S8XOHJhWJAUOYNt-2oQ5lxykY4zsR90tUX4iBBfc)**


### Transition Table
State\Input| 0 | 1 |
--|--|--|
q0 | q0 | q1 | 
q1 | q2 | q1 |
q2 | q2 | q2 |

<hr>

#### Q4. Create the transition function and transition table for the following inputs : 
δ(q~0~,0) = q~0~ 	δ(q~0~,1) = q~2~ δ(q~1~,0) = q~0~ 	δ(q~1~,1) = q~2~ 	δ(q~2~,0) = q~2~ 	δ(q~2~,1) = q~2~ 

Ans. 
### Transition Diagram


**![](https://lh7-us.googleusercontent.com/mnt1NqT8jHnMKPrulOJei4ybpj6QHf1WYRtgLVrb6I18PpM_XVXYEuUoNefe_zDQTHktBCGu97Wbmg4wFIP2ZRKAOfn8wWC_80JWMmItBoJLtsVfvWy4Jyo6PbgL8Jod6tY6FGGm8DUrRI2gdLG3NXU)**


### Transition Table
State\Input| 0 | 1 |
--|--|--|
q0 | q0 | q2 | 
q1 | q0 | q2 |
q2 | q2 | q2 |

<hr>


## Derivation Trees
Derivation tree is a graphical representation for the derivation of the given production rules for a given CFG. 

#### Ex 1.Generate string a*b+c & draw the derivation tree. 
Given Production rules :
1. E = E+E
2. E = E*E
3. E = a/b/c

*Ans*.
**![](https://lh7-us.googleusercontent.com/v0fibVpNCoLPXetvafNpYtr5a7hv91A5YGd_lNu6_qsoRABAwQxgE5RvT225-q8bgFSmIBwDGhNHg6AoEljgOTnglPv5p_i4_M_nAqTzkxuenU6CM7uOka6Csna6UCRDZMaLUMX8hrXeVyoYVkEuqtU)**
<hr>

#### Ex 2.Generate string bbabb or bab & draw the derivation tree. 
Given Production rules :
1. s = bsb
2. s = a
3. s= b

*Ans*.

**![](https://lh7-us.googleusercontent.com/wwKTWYMQzsl97Q9Fb4Zm6bxgCqj5VPr0bVWYROAEx-pCgcPI8Ay7ff9bGPGDz3qIqOiYjrJjgRlCFy0zDhTY5a5HSu0Ay15mdVAN1ys68lvftHhrmXjB9xjjFLyCEweESCBfRG3n338iqFQWn6rNkRY)**

<hr>

#### Ex 3.Generate string aabbabba & draw the derivation tree. 
Given Production rules :
1. s = ab/ba
2. A = a/as/baa
3. B = b/bs/abb

*Ans*.

**![](https://lh7-us.googleusercontent.com/khfllUAKYZqoDsgf5EOPW6xH_ZSNBFaeIvnkQ7RAn8uNeVpwTN2r1cMTEuSStC036Af2Bm1YrHj0UFDsoBHBY-d-9hLBG1Y_QzukSjV1zd1K9KMTvJQo2hRLkZbNvKpmkI7lPMBUG9NAqRC4xcZK2OM)**

#### Ex 4.Generate string aabbbb & draw the derivation tree.  
Given Production rules :
1. s = ab/e
2. a = ab
3. b = sb

*Ans*.

**![](https://lh7-us.googleusercontent.com/hs1nOgYURodMmW5vT--04G1PbTYhsBXQnHcRCvYob1rVmRxQraOiv5mwQj-jVI7k_zquPA5KYhfX3Juu5n30I0jjpEKeL1q-77vZKienX4s5UQqlpVaLWmg5puZ8d-cysQoX0NPTskZFEu6LtWWoq_E)**

<hr>


#### Q. What is Machine Learning, what are the types of machine learning ? Draw the classification tree for types of machine learning.

*Ans* 

**![](https://lh7-us.googleusercontent.com/cAiHLrCGN60cgVcHKEaAWPCUaMqyMTpFQ-EqoijA512lFDSBIkwJjjzjDz9JQjPDmw6YfQeMx0GX4sjw6nkZYg2keBPk2lGCNNBwDyJfjHhSQbHz8U3ILUkdzHrdxGxDKKQtp93BBC2p3MlkDW-1Sfg)**


#### Q. What are the types of SVM ? Draw the classification tree diagram and explain them with graphs. What is Hyper plane and support vector ?

*Ans* Support Vector Machine [SVM] Is a form of classification in *Supervised* machine learning.
* It works best on smaller datasets 
* Can be used for both regression and classification tasks but they work best for classification tasks

In SVM we try to find a hyperplane that best separates the two classes.

**![](https://lh7-us.googleusercontent.com/Ffi0zBT773JE4O3jFSGQTlKRVFYOMPlXwpPilHW3E4LumhlkhHtOlwFu9sge6KwOa5mPquamI6srFaCnOoLUaldwTySBrbAtZKAYZS7avuTTpaqKz-Xnn4U87ko4wMrX_rr0C0lN5TLr1gr3pkFW1k0)**

#### Linear SVM
When the data is perfectly linearly separable only then we can use Linear
SVM.
**![](https://lh7-us.googleusercontent.com/P_o7HoYPGO8Gr1KxrLzIOn1VdMO36CkCNMbxrT538uG6XUK42Ies0x9lMhbT2mUOiK8ZOd7APmYJY-aaHJeZCumOmhCB5wgWdzroQ-9RK5e9r0NrVC0k4k5zAi1q7Aci-r2ZQ9q5UIIG1BDlkmkx8aU)**
**![](https://lh7-us.googleusercontent.com/z6_-zU9R9LR9U_0gmZ9Es--N7XEPDCIfjHzirfWlcpbv2wcV4I3CKdUwmJQ5bjunYYOuR9Vj7fgQcOGA18Ck92WyBO46-KiUHy6gkBGyNqiO3HeFEQMQFcwXfLW7Xc8KjuUx7Qf6QV1jaX-oeXC83cI)**
>  Negative Hyperplane in the image below
**![](https://lh7-us.googleusercontent.com/z6_-zU9R9LR9U_0gmZ9Es--N7XEPDCIfjHzirfWlcpbv2wcV4I3CKdUwmJQ5bjunYYOuR9Vj7fgQcOGA18Ck92WyBO46-KiUHy6gkBGyNqiO3HeFEQMQFcwXfLW7Xc8KjuUx7Qf6QV1jaX-oeXC83cI)**

| Symbol | Name | Meaning | 
|--|--|--|
| ---- |Hyperplane | Straight Line dividing two sets of datapoints|
|*/x | Support Vectors | Data points from different sets, closest to the margins |
| *-/-x | Margin | It is the distance between the support vector and the hyperplane }


#### Non Linear SVM 
When the data is not linearly separable then we can use Non-Linear SVM,
which means when the data points cannot be separated into 2 classes by
using a straight line
**![](https://lh7-us.googleusercontent.com/xX63Wu2C77ye0H4dpRmuYmG8L0POa9FZYLmLLtuwYyb7ORFL2AoTfoJhIptR_2KRDGt2RckF0B_JHogfeWguO37KJfdHi9atRPBH2CqcN8OaWkMDyCAu5ogPKb-wRB57tUevX31_hq0yYVGtpuFqcQ4)**
**Support Vectors**: These are the points that are closest to the hyperplane. A
separating line will be defined with the help of these data points.

**Margin**: it is the distance between the hyperplane and the observations
closest to the hyperplane (support vectors).
<hr>

#### GMM 
GMM is a probabalistic model for representing Gaussian Distribution ( Also known as normal distribution ) and is in a bell shaped curve. It requires statistic values such as mean, standard deviation and such parameters. 
**![](https://lh7-us.googleusercontent.com/po40sfMnraZk4NOhftSZ_bT7TEpuZtqd3ahVyV-mq87azvqfecw5dm30M8inbmMM-_3uJb54CbE_hJ32447Yk_mkInjOZAJvEYdsbP4U1l4t2Dj-edZC68tfW_JqPvWxB3fgguZd8fqErYUUFW5CxIw)**
**![](https://lh7-us.googleusercontent.com/rbAoqaB5OLamb6ElC9zBW_zJYwqdvEsnLZIUtak2y_5-kYuJ7D2TtcIvqTofskl3gmE8Ii3qL21ofYbpWj22e-bE1vaU2cEk9DvXiQRkhq2yVUbNsb5Cfg2brBKHvqGagbs-p3KFY5QqfyQmWgTODYY)**
Where 
u = mean
σ = standard deviation
 x = normal random variable

While modeling human height data, it is typically modelled as a normal distribution for each gender with an approximate mean of : 
5'10" for males and
5'5" for females



