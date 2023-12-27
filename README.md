# Task List Kata

This is a simple Kata for beginner-intermediate level software engineers.

The goal is to create a command line application which allows the creation and listing of a task list.

You should solve this test-first - write tests which capture the acceptance criteria, and make them pass.  You should write unit tests and integration tests to cover both the functions which implement the behaviour of the tool, and the behaviour of the CLI itself, on the command line.  

The suggested time for this is 90-120 mins.  A novice without much experience of Rust's ownership and borrowing system, someone with little to no experience of TDD and BDD, especially in Rust, and someone who has never attempted to build or test a CLI before would not be expected to complete the entire Kata the first time around.  An intermediate or beyond programmer would be expected to have a fully functioning MVP within the time.

This is an ideal task to carry out in a pair or mob - consider rotating the person at the keyboard ever 10 mins.

## Instructions

- Set aside a couple of hours for the kata
- Clone this repo, and move this `README.md` file to `INSTRUCTIONS.md`.
- Create a new `README.md` to document the Kata
- Write an integration test which asserts some expected behaviour of the CLI
- Run it and see it fail
- Write a unit test which will test the required functionality to make the CLI work
- Run it and see it fail
- Write the code to make the unit test pass
- Write any extra code to use the functionality you tested with your unit test, to make the integration test pass
- Repeat!
- When your time runs out, stop, and reflect on and discuss what you learned

## Domain Language

A `task` is a one sentence summary of a discreet action which needs to be taken, for example "wash the dishes".

The `tasklist` is an unordered collection of tasks.

To `add` a `task` is to put it on the list.

## Miniumum Viable Product

The minimum viable product has the following features:

- A task can be added to the task list
- The task list can be shown

Example usage:

```shell
tasklist add make coffee

Added "make coffee" to your task list.

tasklist list

make coffee
```

Your command should respond to and `--help, -h`, to `--version, -v`, and when called without arguments should give a summary of the command and its subcommands.

When called with the `add` command, and no task, it should return help for the add command.


