# Compiler Concepts and Phases

This README outlines the key phases of a compiler and provides a brief explanation of related topics in automata theory, grammars, and parsing.

## Phases of a Compiler

1. **Lexical Analysis**  
   - The process of converting the input text into a series of tokens.
   
2. **Syntax Analysis (Parsing)**  
   - Involves checking the token stream against a formal grammar to build a parse tree.

3. **Semantic Analysis**  
   - Ensures that the parse tree follows the rules of the programming language, ensuring correct meaning.

4. **Intermediate Code Generation**  
   - Translates the high-level language into an intermediate representation (IR).

5. **Code Optimization**  
   - Improves the efficiency of the intermediate code, reducing resource usage.

6. **Code Generation**  
   - Converts the optimized intermediate code into machine code or bytecode.

7. **Code Linking and Loading**  
   - Links various program modules and libraries to create the final executable.

---

## Automata Theory Concepts

1. **Regular Expressions**  
   - Describes patterns used to match strings in lexical analysis.

2. **Finite Automata (FA)**  
   - Used in lexical analysis to recognize tokens:
     - **NFA with ε-transitions**: Allows non-deterministic transitions.
     - **DFA (Deterministic Finite Automaton)**: Used after converting from an NFA for deterministic transitions.

3. **Regex to NFA with ε-transitions**  
   - Converts regular expressions to a non-deterministic finite automaton with epsilon (ε) transitions.

4. **NFA ε-closure**  
   - The set of all states reachable from a state, including ε-transitions.

5. **Rabin-Scott Powerset Construction (NFA to DFA)**  
   - Converts a non-deterministic finite automaton (NFA) to a deterministic one (DFA).

---

## Grammar and Parsing Concepts

1. **Context-Free Grammars (CFGs)**  
   - Defines syntactic structures used in parsing.
   
2. **Ambiguous Grammars**  
   - Grammars that can generate more than one parse tree for a single string.

3. **Fixing Precedence and Associativity in CFGs**  
   - Resolves ambiguity by defining operator precedence and associativity rules.

4. **Backus-Naur Form (BNF)**  
   - A formal notation for context-free grammars used in defining language syntax.

5. **Parse Trees**  
   - A tree representation of syntactic structure following grammar rules.

6. **Syntax-Directed Definitions**  
   - Associates semantic actions with grammar rules to guide translation during parsing.

7. **Syntax-Directed Translation**  
   - Uses syntax-directed definitions to translate input source code into another representation during compilation.
