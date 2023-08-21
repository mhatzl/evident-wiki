# cap: Capturing Events

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 25 (4 direct)

As a user, I want that set events are captured and sent to subscribers, to create an event-driven architecture.

## Active sub-requirements

- [req:cap.ctrl](5-REQ-cap.ctrl)
- [req:cap.filter](5-REQ-cap.filter)

## cap.test.recv: Captured event received by a subscriber

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 1

A set event is sent to a subscriber that is subscribed to this event.

## cap.test.mult: Multiple captured events received by a subscriber

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 1

Multiple set events are received by a subscriber that is subscribed to receive all set events.
