# Chapter 1: What is JavaScript

## *What's With That Name?*

* JavaScript's name is a marketing ploy. Brandon Eich named it Mocha; Netscape called it LiveScript; JavaScript was meant to make it palatable to Java developers since the word 'script' was popular at the time. Script referred to lightwieght programs that would load on this "new" Internet.
  
* Superficial resemblance to Java

  * Both have C synatx expectation (ex. using `{` & `}` to begin & end code blocks)

* Oracle (owner of Java) owns the JavaScript trademark via NetScape

* Typically use JS instead of JavaScript

* Official language name is ECMAScript followed by the revision year (ECMAScript2019/ES2019)

> "Java is to JavaScript as ham is to hamster." --Jeremy Keith, 2009

## *Language Specification*

* TC39 - official steering committee that manages JS.

  * Manage the official specification
  
  * Meet to vote on agreed changes and submit them to ECMA (the standards org.)

  * Comprised of between 50 and about 100 different people from a broad section of web-invested companies (Google, Apple, Mozilla, Samsung, etc)

* 5 stage process for proposals:

  * Stage 0
    * TC39 member thinks it's worthy and champions it
    * Non-TC39 make suggestions via social media platforms (pre-stage 0)
  * Stage 1
  * Stage 2
  * Stage 3
  * Stage 4
    * Eligible to be included in the next yearly revision
  * Can take months to years to go from 0-5

* **Only one JS that is managed and maintained by TC39/ECMA**

  * All browsers/devices agree to keep their JS implementation compliant with that one specification

### The Web Rules Everything About (JS)

* The Web is king when it comes to JS. For the most part, the JS spec matches the JS run in the browser. But browser based JS engines won't conform to spec changes if doing so will break the web content.
  
### Not All (Web) JS...

* `alert("Hello, JS!");` The `alert` function is not part of the JS spec, but many JS environments add APIs that enhance JS functionality. The Web APIs look like JS, but are not defined in the JS specification. The `alert(...)` call is JS, but `alert` is not.
* 
### It's Not Always JS

* Console/REPL (Read/Evaluate/Print/Loop) isn't a pure JS environment. 

  * It's a tool for developers to make their life easier.
    
  * Prioritizes Developer Experience(DX) 
    
  * Doesn't always exactly adhere to how a program would actually run

  * **Key Takeaway:** Console behavior doesn't always represent exact to-the-letter JS semantics
  
## *Many Faces*

**Paradigm**: broad/universal mindset & approach to structuring code

* **Procedural**

  * Orgainzed top-down, linear progression through a set of operations that are called together (procedures)

* **Object-oriented** (OO/classes)

  * Puts data and logic into units (classes)

* **Functional** (FP)

  * Organized by functions and uses how those functions change as values

* No right or wrong paradigm. Just guides how you approach problems/solutions. And how you structure/maintain your code

* Some languages slant in a particular direction:

  * C -> procedural

  * Java/C++ -> OOP

  * Haskel -> FP

* Multi-paradigmed languages offer flexibility -> JS is multi-paradigmed

## *Backwards & Forwards*

* JS is, and must be, **backwards-compatible**:

  * Once a spec is accepted, it can never be invalid. 

* JS developers are assured that their code will always work as designed, making JS a safe choice for web programming.

* JS is **NOT** ***forward-compatible*** (ensuring that new code can run in old environments without breaking) 

* HTML/CSS is forward-compatible (new HTML/CSS can run in old browsers without breaking it)
  
* Browsers can can skip over HTML/CSS declarations it might not understand, but a program can't skip over declarations with causing chaos.

### Jumping the Gaps

* Transpiling converts code from one form to another. 

* Used to solve forward-compatibility problems.

* Transpiler are usually used to solve forward-compatabilty syntax issues
  
| NOTE: |
| :--- |
| JS developers should use the latest implementation of JS so code is clean and easy to understand

### Filling the Gaps

* Polyfills are used to solve forward-compatibility isses not realted to syntax errors (ex. missing API methods)
  
## *What's in an Interpretation?*

* Debate: JS, interpreted script or compiled program?

  * Scripting languages: 
    * Use dynamic typing 
    * Distribute the source code (not the binary form)
    * Executed top down, line by line
    * Not parsed before executed
  
  * Compiled programs:
    * Ise static typing
    * Represent the program as binary before execution
  
  * Parsed languages;
    * Parsed & compiled before execution (transformed into en executable form)
    * All compiled languages are parsed
    * JS is parsed before execution
      * Calls for early errors:
        * Recognizing duplicate parameter names, so it is paresed before execution
  
  * Is JS compiled?
    * More yes than no
      * Parsed JS is converted to binary and doesn't switch back to line-by-line execution (very inefficient)
      * The binary code is execute by the JVM

  * Flow of JS program
    1. Transpiled * packed (Babel & WebPack) and handed to the JS engine in a form different from which it started
    2. JS engine parses the code to an **Abstract Syntax Tree (AST)** - executable
    3. JS engine converts the AST -> binary intermediate representation -> optimized by **Just-In-Time (JIT)** compiler
    4. JVM runs the program

| Takeaway: |
| :--- |
| In spirit, if not in practice, JS is a compiled language.
  
### Web Assembly (WASM) 

* How fast JS can parse & execute a program is a big concern 
* **ASM.js** 
  * Used to transpile Unreal 3 game engine (written in C) to JS
  * written in uncommon form -> signal typing info for optimization
  * Addresses some of that concern
  * Shows that JS could be used to create transpiled versions of programs that ran more effciently
* **WASM**
  * Used to convert non-JS programs to be able to run on the JS engine, but also get by the delays caused by parsing/compiling -> represents the program in an unlike JS form
  * Way to bring more non-JS programs to web platforms
  * Relieves the pressure to add features to JS that are mostly/exclusively intended to be used by transpiled programs from other languages. 
  * WASM is evolving to become a cross-platform virtual machine (VM) of sorts, where programs can be compiled once and run in a variety of different system environments.

| Takeaway: |
| :--- |
| WASM significantly augments what the web (including JS) can accomplish

  
## *Strictly Speaking*

* Use strict mode: `"use strict";`
  * Guide to the best way to do things (helps the optimizatiom & efficiency of code)
  
## **Defined**
**JavaScript**
: JS is an implementation of the ECMAScript standard (version ES2019 as of this writing), which is guided by the TC39 committee and hosted by ECMA. It runs in browsers and other JS environments such as Node.js.

JS is a multi-paradigm language, meaning the syntax and capabilities allow a developer to mix and match (and bend and reshape!) concepts from various major paradigms, such as procedural, object-oriented (OO/classes), and functional (FP).

JS is a compiled language, meaning the tools (including the JS engine) process and verify a program (reporting any errors!) before it executes.

With our language now defined, let's start getting to know its ins and outs.