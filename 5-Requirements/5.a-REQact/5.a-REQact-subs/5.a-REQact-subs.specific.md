# subs.specific: Subscribe to specific events

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

As a user, I want to be able to subscribe to specific events, because I am either only interested in certain events, or because I want to react differently depending on the received event.

**Implementation Details:**

Since events are identified using an event-ID, this ID must be used for subscriptions.

## subs.specific.one: Subscribe to one specific event

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

*evident* must provide a function to subscribe to one specific event.

### subs.specific.one.test.recv: Receive event the subscriber is subscribed to

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

Set event is received by the subscriber that only subscribed to this event.

### subs.specific.one.test.ignore: Subscriber does not receive events that are not subscribed

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

Set event not subscribed by the subscriber. The subscriber must not receive this event.

## subs.specific.mult: Subscribe to multiple specific events

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

*evident* must provide a function to subscribe to multiple specific events at once.

### subs.specific.mult.test.recv: Receive multiple subscribed events

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

Multiple events the subscriber is subscribed to are received.

## subs.specific.mult.test.ignore: Subscriber ignores events that are not subscribed

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

Only events that are subscribed are received by the subscriber, and all other events are ignored.
