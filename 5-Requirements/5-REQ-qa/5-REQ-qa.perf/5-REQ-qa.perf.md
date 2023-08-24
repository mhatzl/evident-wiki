# qa.perf: Performance considerations

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 1 (0 direct)

The performance penalty for using *evident* should be as low as possible.
Especially lowering the performance penalty for capturing events should be prioritized over other areas, because capturing most likely happens during execution of business logic.

## Sub-requirements

- [req:qa.perf.locks](5-REQ-qa.perf.locks)
