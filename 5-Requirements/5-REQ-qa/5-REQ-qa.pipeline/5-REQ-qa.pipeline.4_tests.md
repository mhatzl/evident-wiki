# qa.pipeline.4_tests:

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 1

`cargo test` is used to run all *evident* tests.

## Implementation Details

`cargo test -- --test-threads 1` is used, because tests cannot be run in parallel as tests use the same events and publisher.
