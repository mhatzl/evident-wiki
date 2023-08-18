# qa.ux: User experience considerations

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

*evident* should be easy to set up basic pub/sub functionalities, while allowing enough flexibility to customize the event data that is sent.

## qa.ux.macros: Use macros if it improves usability

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

Rust macros may be used if they improve the usability of *evident*.
However, IDE support for macros is not as good as for functions, so wherever possible try to use functions instead of macros.

## qa.ux.usage: Provide usage examples

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

Usage examples help users to better understand how to use particular functionalities of *evident*. 
Especially common or complex functionalities should have usage examples in their doc-comments.
