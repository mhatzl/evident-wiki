# qa: Quality Assurance

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

*QA* requirements help to ensure a high quality for *evident*.

**Note:** General *QA* requirements affect the overall architecture and implementation of *evident*, because they are not specific to a feature/functionality. Therefore, these requirements must be considered for every existing or new feature/functionality, as long as these *QA* requirements are *active*.

**Note:** Only general *QA* requirements should be part of this requirement group. *QA* requirements that are specific to a requirement group should be added to a *qa* requirement subgroup for this feature.

## qa.DoD: Have a "Definition of Done" for requirements

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main):

A "Definition of Done" is used to ensure consistent quality for new implementations.
Issues may add additional content to the general "Definition of Done".

## qa.DoR: Have a "Definition of Ready" for requirements

A "Definition of Ready" is used to define, when a requirement may be moved from *proposed* to *ready*.

## qa.links: Use requirement tags in the *evident* repository

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main):

Requirement tags should be set in the *evident* repository at file locations, where the requirement is implemented,
or where it affected the design of the implementation.
Tags must be set using the syntax `[req:my.tag]`, with an optional link added with `[req:my.tag](URI to requirement)`.

**Note:** This helps with traceability between requirements and implementation.

## qa.perf: Performance considerations

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

The performance penalty for using *evident* should be as low as possible.
Especially lowering the performance penalty for capturing events should be prioritized over other areas, because capturing most likely happens during execution of business logic.

### qa.perf.locks: Performance impact of multithreaded locking

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

Use as few write-locks as possible, and prefer `RwLock` over `Mutex`.

**Note:** `RwLock` allows multiple read-locks on the same shared data.

## qa.sustain: Consider sustainability during design and development

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

Sustainability is becoming more and more important.
Therefore, sustainability should be considered during design decisions and development of *evident*.

**Note:** Also during development, because e.g. CI/CD-pipelines may unnecessarily waste resources.

## Other active sub-requirements

- [req:qa.pipeline](5-REQ-qa.pipeline)
- [req:qa.ux](5-REQ-qa.ux)
