# qa.links: Use requirement tags in the *evident* repository

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main):

Requirement tags should be set in the *evident* repository at file locations, where the requirement is implemented,
or where it affected the design of the implementation.
Tags must be set using the syntax `[req:my.tag]`, with an optional link added with `[req:my.tag](URI to requirement)`.

**Note:** This helps with traceability between requirements and implementation.
