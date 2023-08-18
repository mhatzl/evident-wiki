# pub: Event publishing

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

As a user, I want that captured events are published to subscribers of the event, to create an event-driven architecture.

## Implementation Details

A central *publisher* is used to capture all set events, and then forward those events to the subscribers that are subscribed to those events.
For more information, see [DR-20230809_2](6-DR-20230809_2).

## pub.threaded: Multithreaded publishing

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

As a user, I want to be able to set events in multiple threads, and be able to have multiple subscribers in other threads receiving these events, because I want to be able to asynchronously react to events.

### pub.threaded.test: Events set in multiple threads received by subscriber

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

**Steps:**

1. Create a subscriber for all events
1. Set multiple events in different threads
1. All events are received by the subscriber
