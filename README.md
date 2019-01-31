# RUST

Rust is a fairly new language derived from the Mozilla Foundation. 
https://www.rust-lang.org/


---



# What is RUST?

Rust is a systems programing language that runs blazing fast, prevents almost all crashes, and eliminates data races.

Rust is known as a systems programming language. 

Systems programming language provides the following:



*   Fine grained control over allocations
*   No required garbage collector
*   Minimal runtime
*   Close to the metal (hardware abstraction layer)


# Why rust?


### Let's compare!

C/C++ = More control yet, less safety

Java = Middle ground between safety and control

Python = Less control yet, more safety

Rust = More control with safety :) 


### Rust runs blazingly fast!



*   Compiles to an executable binary
*   LLVM backend
*   LLVM suite of optimizations
*   Competitive with C/C++


### Rust prevents 'almost' all crashes



*   Safe by default
*   Sophisticated type system and analysis
*   No Segfaults
*   No null pointers
*   No dangling pointers


### Eliminates data races



*   Ownership guarantees
*   Borrowing prevents dangling pointers
		*   Borrowed values can be owned through cloning.
*   Strong and safe abstractions
*   Concurrency using ownerships prevents data race (similar to GO)


# So who is using RUST?


### Rust is using Rust!



*   92% Rust
*   3.6% C - bundled libraries
*   1.6% bash
*   3% others?


### Servo



*   Parallel layout engine for web to render HTML from the ground up.


# Concerns

The mature languages offer strong support for developers looking to focus on business growth or discovering employment opportunities.  At the moment, Rust is great for exploratory efforts and testing. Albeit, as it matures and more companies depend on Rust in production the language will offer similar benefits as seen today with mature languages. Example: GoLang took 4 years to take off and establish itself as the goto for backend services. Similar experience with Kotlin. Once adoption took place, developers in these new languages became in high-demand. 


# What is the true problem that Rust is trying to solve? 

It seems the focus is on performance, reliability, and memory efficiency. 

Let's take a peak at the differences with web development and look at the reasons why to use Rust over Javascript.

- Performance boost x6

- Typings

- Smart compiler

- Predictable memory control﻿

- Reliablity

On the note of web development, Javascript is easier to write versus Rust. Outside web development, Rust is known to perform well with kernel development. IoT seems to be a stongsuite with Rust and will mature well within that space. 


# Getting started with Development

Install Rust tooling: [https://www.rust-lang.org/tools/install](https://www.rust-lang.org/tools/install)

```

curl https://sh.rustup.rs -sSf | sh

```

Note: Installing Rust tools might prompt you to modify your environment paths. This is typical and often neglected as a warning upon installations with other languages which often means the developer would need to adjust the environment paths. It's nice to see Rust provides insight right from the start. Furthermore, Rust makes sure you understand that the modifications to your paths can be reverted utilizing 'rustup self uninstall' command. If prompted and you don't know what to select, just press enter to accept default option to proceed with installation.


### Part 1: Hello World

Create a new directory for the project

Create a new file within the project directory called main.rs

Within main.rs create a new function called main(){}. Like many other languages Rust depends on the main() function for it's starting point with your application.

Defining a function utilizes fn syntax followed by the function name. In the example below, we define the main() function with no arguments. The main() function body issues the println command followed by text to be returned.

```

Fn main() {

	println!("Hello, World!");

}

```

Executing the application

Utilizing a terminal, make sure to navigate the terminal to the project directory. Next, compile the application using the rust compiler.

Example:

rustc main.rs


### What about project and package management ?

Other languages typically have dependency managers, for instance, Javascript with Node.js utilizing NPM. Rust has a similar option called Cargo. Let's experiment and create a new project with Cargo.

In a new terminal window navigate to your projects working directory.

Issue the command:

```

cargo new hello-world --bin

```

Using --bin flag tells cargo that the project is an binary executable versus a library. Without the --bin flag cargo will default to library project.

A new directory for your project will be created, take a look at the files. Similar to NPM, Cargo creates the following files to help manage your project:

Cargo.toml - Package configurations file for your project along with dependency list

.git - default configuration for git repo

.gitignore - Pre-made git ignore file to prevent junk from pushing to your GitHub project repo

Src directory - Directory containing your source files

To execute a program using cargo, navigate to your project directory in a terminal window and type 'cargo run'. Cargo will compile the project and execute.


### Comments in Rust

Single line comment = // comment

Multi-line comment = /* multi-line comment */
