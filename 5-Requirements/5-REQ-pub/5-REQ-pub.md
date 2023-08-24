# pub: Event publishing

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 6 (4 direct)

As a user, I want that captured events are published to subscribers of the event, to create an event-driven architecture.

## Implementation Details

A central *publisher* is used to capture all set events, and then forwards those events to the subscribers that are subscribed to those events.
For more information, see [DR-20230809_2](6-DR-20230809_2).

## Sub-requirements

- [req:pub.threaded](5-REQ-pub.threaded)
