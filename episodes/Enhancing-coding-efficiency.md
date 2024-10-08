---
title: "Enhancing Coding Efficiency"
teaching: TBD
exercises: TBD
---

:::::::::::::::::::::::::::::::::::::: questions 

- How can the autocomplete function in Codeium help improve your coding speed?
- What types of repetitive coding tasks can be automated?
- What are some key components of a clear and effective prompt when using the autocomplete function?
- In what ways can Codeium assist in generating and improving code documentation?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Use an autocomplete function of Codeium to improve coding speed
- Automate repetitive coding tasks using the autocomplete function of Codeium
- Compose clear and effective prompts that capture and facilitate the expected outcomes using the autocomplete function
- Generate and improve documentation using Codeium

::::::::::::::::::::::::::::::::::::::::::::::::

## Autocomplete Function

A key feature of Codeium is its autocomplete function: with every keystroke, Codeium actively attempts to predict and complete what you're typing. By analyzing the current file, previous edits, and contextual snippets from your codebase, it offers relevant suggestions as "ghost text".

![](episodes/fig/acceleration.gif){alt='Autocomplete Function'}

This feature can be particularly useful when you're writing repetitive code or boilerplate, as it can save you time and reduce the likelihood of errors. By leveraging Codeium's autocomplete function, you can speed up your coding process and focus on the more creative and challenging aspects of your work.

### Boilerplate, Formatting, and More

As already mentioned above, one of the most powerful ways to use Codeium is for automating repetitive coding tasks. Whether you’re writing boilerplate code, standard functions, or common design patterns, Codeium's AI assistant can help speed up the process and reduce the manual effort required.

By recognizing patterns in your codebase, Codeium can predict and suggest repetitive structures such as:

- **Boilerplate code**: Generate routine code structures like class definitions, function signatures, or common initialization blocks with minimal effort.
- **Repetitive functions**: Quickly replicate commonly used functions or methods that follow a similar pattern, reducing the need for retyping or copy-pasting.
- **Code formatting and styling**: Maintain consistency in your code format by allowing Codeium to suggest and automate repetitive formatting tasks, saving you from manual corrections.

For example, when writing a set of functions that handle similar operations, Codeium can recognize the pattern after a few examples and suggest the next method based on prior code. This not only speeds up your workflow but also minimizes the risk of errors from copying or manually creating repetitive code.

### Fill-in-the-middle (FIM)

Codeium's Autocomplete model also includes Fill-in-the-Middle (FIM) capabilities. This is crucial because, more often than not, you're inserting code within an existing file, rather than just appending new lines. With FIM, Autocomplete analyzes the code both above and below the current line to provide more accurate suggestions.

Let's compare the FIM-enabled model to the standard model.

Codeium Autocomplete (with FIM):

![](episodes/fig/fim_12.png){alt='FIM'}

Competitor Autocomplete (without FIM): 

![](episodes/fig/fim_13.png){alt='No FIM'}

Note that the non-FIM model suggests a generic docstring based on only the preceding line with the function signature. In contrast, the FIM model provides a more contextually relevant suggestion based on the entire function definition.

### Inline Comments

You can guide the autocomplete feature by using comments within your code. Codeium interprets these comments and generates code suggestions to implement what the comment describes.

![](episodes/fig/minimize_boilerplate.gif){alt='Inline Comments'}

### Shortcuts

The following shortcuts can be used to speed up your workflow: 

- `Tab` = accept suggestion
- `Cmd` + `Left Arrow` = accept next word in suggestion
- `Option` + `]` = next suggestion
- `Esc` = clear suggestions 

### Best Practices

- Avoid manually triggering autocomplete; instead, let it naturally enhance your workflow. Writing prompts as comments is not recommended, but decorating your code with quality comments and information variable/function names yields the best results.
- To achieve the best results with autocomplete, it's important to enhance your code with clear, *declarative* (not instructive) code, descriptive function names, and good comments with examples of the desired inputs and outputs. See the table below for examples:

    ![](episodes/fig/table_autocomplete.png){alt='Best Practices for Autocomplete'}

- If needed, you can temporarily snooze autocomplete. This feature is available in VS Code version 1.8.66. Simply click the Codeium button in the bottom right to access it.

## Documentation Generation

Codeium displays code lenses, which are small, clickable text labels, above functions and classes. These lenses allow you to easily invoke Codeium’s AI capabilities for the specific item they reference.

In the [previous episode](add link), we explored the `Refactor` code lens. Now, let’s focus on the `Docstring` lens.

When you click on `Docstring`, Codeium will automatically generate a docstring above the function header. In Python, the docstring will be correctly placed directly beneath the function header.

![](episodes/fig/jetbrains_docstrings.mp4){alt='Docstring generation'}

::::::::::::::::::::::::::::::::::::: challenge 

TODO

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: keypoints 

- Codeium's autocomplete boosts coding speed by predicting and completing code based on context, past edits, and current files.
- Automating repetitive tasks like boilerplate code, repetitive functions, and formatting reduces errors and saves time.
- Fill-in-the-Middle (FIM) improves suggestions by analyzing the code above and below the insertion point.
- Docstring generation via code lenses automates the creation of accurate docstrings in the correct location.

::::::::::::::::::::::::::::::::::::::::::::::::
