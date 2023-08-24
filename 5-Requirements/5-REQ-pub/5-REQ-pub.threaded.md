# pub.threaded: Multithreaded publishing

**References:**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 2 (1 direct)

As a user, I want to be able to set events in multiple threads, and be able to have multiple subscribers in other threads receiving these events, because I want to be able to asynchronously react to events.

## pub.threaded.test: Events set in multiple threads received by subscriber

**References:**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 1

**Steps:**

1. Create a subscriber for all events
1. Set multiple events in different threads
1. All events are received by the subscriber
