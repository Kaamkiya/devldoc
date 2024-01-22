# Using devl

If you haven't already [installed devl](/dl), do that first.

## Adding to $PATH
To get started with devl, first make sure that the executable is in your path.
This allows you to use it just by typing `devl` instead of `/path/to/devl`.

If you installed with the Go CLI, run this in your shell:
```bash
export PATH="$PATH:$HOME/go/bin"
```

If you installed with curl, do this:
```bash
export PATH="$PATH:$HOME/.devl"
```

## Getting started

Type the following command into your terminal/command prompt:
```bash
devl
```

That should output a message on how to use it.

Now try this:
```bash
devl help
```

That will output a much more detailed and descriptive explanation of how to use
it. If you like getting your hands dirty, play with the tips it gives you.

Here's the rest anyway.

## devl help

This prints a help message, as we saw above.

If you put something after the `help` parameter, it prints help for that, or 
gives you an error message.

## devl quiz

This command will quiz you on whatever you like. To see all of the quizzes, 
type this command:

```bash
devl help quiz
```

This should print how to use it and list all available quizzes.

When you type this command (with and argument), a question will be printed.
You can then enter your answer, in the form of a letter. **Beware**, though,
that the input you give is not verifiead, so it'll just be considered wrong.

Use this command to get quizzed:
```bash
devl quiz <language>
```

Try it!

## devl resource

This command provides a list of resources for whatever you enter. This is 
probably the best and easiest thing to contribute to, so make a PR and add some
resources to resources.json!

To learn about the command, type this:
```bash
devl help resource
```

That'll print how to use it.

To try it, type this:
```bash
devl resource go
```

That should output a list of resources about the Go coding language.

To use it in the future, type the following:
```bash
devl resource <thing>
```

Where `<thing>` is whatever you need help with.

Some other examples:
```bash
devl resource oop      # provide resources explaining OOP
devl resource vuejs
devl resource c++
```

## devl cheatsheet

This fetches a cheatsheet and prints it. It currently gets the sheets from
[Learn X in Y minutes](https://learnxinyminutes.com/). 

If it exists in the 
[LearnXinYminutes repo](https://github.com/adambard/learnxinyminutes-docs), you
can just type the following:

```bash
devl cheatsheet <language>
```

Some examples:
```bash
devl cheatsheet c++
devl cheatsheet asymptotic-notation
```
