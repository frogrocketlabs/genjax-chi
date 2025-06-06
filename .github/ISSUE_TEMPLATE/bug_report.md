---
name: Bug report
description: >-
  Report a bug or unexpected behavior to help us improve the package
labels:
- bug

body:
- type: markdown
  attributes:
    value: >
      ## Thank you for helping us improve JAX!

      * Please first verify that your issue is not already reported using the
      [Issue search][issue search].

      * If you prefer a non-templated issue report, click [here][Raw report].

      [issue search]: https://github.com/ChiSym/genjax/search?q=is%3Aissue&type=issues
      [Raw report]: http://github.com/ChiSym/genjax/issues/new

- type: textarea
  attributes:
    label: Description
    description: >-
      A concise description of the bug, preferably including self-contained
      code to reproduce the issue.
    placeholder: |
      Text may use markdown formatting.
      ```python
      # for codeblocks, use triple backticks
      ```
  validations:
    required: true

- type: textarea
  attributes:
    label: System info (python version, jaxlib version, accelerator, etc.)
    description: >-
      Include the output of `import jax; jax.print_environment_info()`
      and `import genjax; print(genjax.__version__)`
    placeholder: |
      ```
      ...
      ```
  validations:
    required: true
