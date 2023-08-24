# cap.ctrl.start: Start Capturing

**References:**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 4 (4 direct)

As a user, I want to be able to start capturing, because I want to resume capturing after manually stopping it for a certain period.

## Implementation Details

Capturing is started by sending a special *start-event* to the event handler, because the handler only reacts to events.
For more information, see [DR-20230809_1](6-DR-20230809_1).

## cap.ctrl.start.test: Events captured after capturing is started again

**Steps:**

1. Create subscriber for all events
1. Manually stop capturing
1. Set first event
1. Manually start capturing
1. Set second event
1. **Check:** Subscriber **only** received second event
