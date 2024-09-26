## BBM 301 - Programming Languages: A Detailed Summary of Week 1

**I. General Information**

* **Course Webpage:** http://web.cs.hacettepe.edu.tr/~bbm301
* **Textbook:** "Concepts of Programming Languages," 12th Edition (11th acceptable) by Robert W. Sebesta 
* **Time and Place:** Thursdays, 09:40 - 12:30 
* **Communication:** Piazza - https://piazza.com/hacettepe.edu.tr/fall2024/bbm301
* **Grading:**
    * 30% Midterm Exam 1
    * 30% Midterm Exam 2
    * 40% Final Exam

**II. Course Topics**

* Introduction to Programming Languages
* Names, Bindings, and Scope
* Syntax and Semantics
* Regular Expressions
* Functional Languages
* Data Types
* Expressions, Assignments, and Control Statements
* Subprograms and their Implementation
* Logic Languages

**III. Why Study Programming Languages?**

* **Broader Skillset:** Knowing one or two languages is insufficient for a well-rounded computer scientist.
* **Underlying Concepts:** Understanding the principles behind language design provides a deeper understanding of programming as a whole.
* **Informed Choices:** Knowing the strengths and weaknesses of different languages allows for better selection of the right tool for the task.

**IV. The Ever-Evolving Landscape of Programming Languages**

* **Abundance of Languages:** There are over 700 programming languages in existence, with new ones constantly being created.
* **Continual Evolution:** Languages undergo constant changes and updates. FORTRAN, ALGOL 60, C, C++, and Java exemplify this evolution.
* **Adapting to Shifts:**  Understanding current computational trends (e.g., the shift toward web-based applications and distributed systems) helps anticipate future language developments.
* **Thought-Shaping Languages:** Alan Perlis famously said, "A language that doesn't affect the way you think about programming is not worth knowing." This course will expose students to unconventional languages like Prolog, which challenge traditional programming paradigms.

**V. Reasons for Studying Programming Language Concepts**

* **Increased Ability to Express Ideas:**
    * **Natural Languages:** The richness of a language influences the depth of thought and communication. Programming languages share this trait.
    * **Programming Languages:** Exposure to diverse language features broadens a programmer's ability to conceptualize and solve problems. 
* **Improved Background for Choosing Appropriate Languages:**
    * **Understanding Trade-offs:** Not all languages are created equal. Different languages excel in different domains (e.g., Perl for text processing, MATLAB for matrix operations).
    * **Informed Decisions:** Familiarity with language principles allows for a reasoned evaluation of language strengths and weaknesses in the context of a specific project. 
* **Increased Ability to Learn New Languages:**
    * **Common Concepts:** Understanding fundamental language concepts makes learning new languages easier. (e.g., knowing object-oriented programming eases the transition from Java to C++).
    * **Enhanced Understanding:** Learning new languages often reinforces the understanding of previously learned ones.

**VI.  Language Evaluation Criteria**

Four main criteria are used to evaluate programming languages:

1. **Readability:** 
    * **Definition:** How easily a program can be read and understood.
    * **Contributing Factors:**
        * Overall Simplicity:  A manageable set of features and minimal feature multiplicity (avoiding multiple ways to achieve the same result). 
        * Orthogonality:  A small set of primitive constructs that can be combined in a consistent and predictable way.  
        * Control Statements: Clear and intuitive control flow mechanisms.
        * Data Types and Structures: Well-defined and easy-to-understand data representations.
        * Syntax Considerations:  Meaningful keywords, consistent formatting, and clear delimiters. 
2. **Writability:** 
    * **Definition:** How easily a language can be used to create programs.
    * **Contributing Factors:**
        * Simplicity and Orthogonality (as defined above).
        * Support for Abstraction: Ability to define and use complex structures and operations while hiding unnecessary details (e.g., subprograms and data structures).
        * Expressivity:  Providing convenient and concise ways to express computations (e.g., powerful operators and built-in functions).
3. **Reliability:**
    * **Definition:** A language's ability to perform according to its specifications under all conditions.
    * **Contributing Factors:**
        * Type Checking: Detecting type errors either during compilation or execution.
        * Exception Handling:  Mechanisms for gracefully handling runtime errors.
        * Aliasing:  The presence of multiple ways to refer to the same memory location, which can lead to unintended side effects.
        * Readability and Writability:  Well-written and easily understood code is more likely to be correct.
4. **Cost:**
    * **Definition:**  The total cost associated with a language, encompassing various factors.
    * **Contributing Factors:**
        * Training: The cost of training programmers to use the language.
        * Writing Programs: The effort required to write programs in the language.
        * Compilation: The cost of the compiler and the time it takes to compile programs.
        * Execution: The resources (e.g., time and memory) needed to execute programs.
        * Implementation System: The cost of the tools and infrastructure required to support the language.
        * Reliability:  The cost of failures and the need for rigorous testing in critical systems.
        * Maintenance:  The cost of correcting, modifying, and updating programs over time, often the most significant expense. 

**VII. Additional Evaluation Criteria**

* **Portability:** The ease of moving programs between different implementations and platforms.
* **Generality:**  A language's applicability to a wide range of problems and domains.
* **Well-Definedness:** The completeness and clarity of the language's official definition.

**VIII. Language Design Trade-offs**

* **Reliability vs. Cost of Execution:** Enforcing strong type checking (as in Java) improves reliability but can increase execution overhead.
* **Readability vs. Writability:** Languages like APL prioritize conciseness and expressiveness, potentially sacrificing readability.
* **Writability (Flexibility) vs. Reliability:** Features like C++ pointers offer flexibility but increase the risk of memory-related errors.

**IX. Language Categories**

* **Imperative:**  Based on variables, assignments, and iteration. Includes object-oriented, scripting, and visual languages. Examples: C, Java, Perl, Visual BASIC .NET, C++.
* **Functional:** Computation primarily achieved by applying functions to arguments. Examples: LISP, Scheme, ML, F#.
* **Logic:** Rule-based, with rules specified without a particular order. Example: Prolog.
* **Markup/Programming Hybrid:** Markup languages extended for programming. Examples: JSTL, XSLT.

**X. Implementation Methods**

* **Compilation:**  Translating programs directly into machine code. Can include Just-In-Time (JIT) compilation. Suited for large, performance-critical applications.
* **Pure Interpretation:** Programs are executed line by line by an interpreter. Good for small programs or when efficiency is not a primary concern.
* **Hybrid Implementation Systems:** Combine elements of compilation and interpretation. Often used for small to medium-sized systems where a balance between performance and development speed is desired.

**XI. Summary**

* Studying programming languages offers significant benefits, including enhanced problem-solving abilities, informed language selection, and easier learning of new languages.
* Readability, writability, reliability, and cost are key criteria for evaluating languages.
* Understanding design trade-offs and language categories provides a broader perspective on the programming landscape.
