# cap.ctrl.stop: Stop Capturing

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

As a user, I want to be able to stop capturing, because I might not want to capture events all the time.

## Implementation Details

Capturing is stopped by sending a special *stop-event* to the event handler, because the handler only reacts to events.
For more information, see [DR-20230809_1](6-DR-20230809_1).

## cap.ctrl.stop.test: Events not captured while capturing is stopped

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

**Steps:**

1. Create subscriber for all events
1. Manually stop capturing
1. Set any event
1. **Check:** Subscriber did **not** receive any event 
