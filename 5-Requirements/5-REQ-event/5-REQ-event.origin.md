# event.origin: Get the event origin

**References:**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 11 (8 direct)

As a user, I want to know the crate, module, and line number the event was set at, because this enables more filter options.

## Implementation Details

Macros must be used to get the event origin directly without user interaction.

## event.origin.test.basic: Origin of set event points to `set_event!()` call

**References:**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 1

The origin of an event points to the code location where the `set_event!()` macro was called.

## event.origin.test.two_origins: Origin of an event set with two `set_event!()` calls differs

**References:**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 1

The origin differs for every call of `set_event!()` not in the same line, even if the event is the same.

## event.origin.test.same_origin: Set origin of an event manually for two `set_event_with_msg()` calls

**References:**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 1

Set the same origin manually for an event that is set two times at different locations.
