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

  * Orgainzed top-down, linear progression through 

* **Object-oriented** (OO/classes)

* **Functional** (FP)
## *Backwards & Forwards*
### Jumping the Gaps
### Filling the Gaps
## *What's in an Interpretation?*
### Web Assembly (WASM) 
## *Strictly Speaking*
## **Defined*