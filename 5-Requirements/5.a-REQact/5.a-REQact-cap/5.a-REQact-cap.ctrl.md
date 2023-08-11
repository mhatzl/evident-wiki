# cap.ctrl: Control Capturing

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

As a user, I want to start and stop capturing during runtime, because I might not want to capture events during certain operations.

## cap.ctrl.init: Initial Capturing State

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

As a user, I want that capturing is active per default, otherwise, every library user would need to start capturing manually. 

### cap.ctrl.init.test: Capturing is turned on by default

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

Events are captured without manually starting capturing.

## cap.ctrl.stop: Stop Capturing

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

As a user, I want to be able to stop capturing, because I might not want to capture events all the time.

### Implementation Details

Capturing is stopped by sending a special *stop-event* to the event handler, because the handler only reacts to events.
For more information, see [DR-20230809_1](6-DR-20230809_1).

### cap.ctrl.stop.test: Events not captured while capturing is stopped

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

**Steps:**

1. Create subscriber for all events
1. Manually stop capturing
1. Set any event
1. **Check:** Subscriber did **not** receive any event 

## cap.ctrl.start: Start Capturing

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

As a user, I want to be able to start capturing, because I want to resume capturing after manually stopping it for a certain period.

### Implementation Details

Capturing is started by sending a special *start-event* to the event handler, because the handler only reacts to events.
For more information, see [DR-20230809_1](6-DR-20230809_1).

### cap.ctrl.start.test: Events captured after capturing is started again

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

**Steps:**

1. Create subscriber for all events
1. Manually stop capturing
1. Set first event
1. Manually start capturing
1. Set second event
1. **Check:** Subscriber **only** received second event

## cap.ctrl.info: Get Capturing-State

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

As a user, I want to know if capturing is active or not, because I want to stay informed about the capturing state.

### cap.ctrl.info.test.init: Capturing is active initially

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

Capturing is active initially: `is_capturing()` returns `true`.

### cap.ctrl.info.test.stop: Capturing is stopped

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

After capturing is stopped, `is_capturing()` returns `false`.

### cap.ctrl.info.test.start: Capturing is started after being stopped

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

After capturing is started again, `is_capturing()` returns `true`.
