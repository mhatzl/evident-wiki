# cap.ctrl.info: Get Capturing-State

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

As a user, I want to know if capturing is active or not, because I want to stay informed about the capturing state.

## cap.ctrl.info.test.init: Capturing is active initially

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

Capturing is active initially: `is_capturing()` returns `true`.

## cap.ctrl.info.test.stop: Capturing is stopped

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

After capturing is stopped, `is_capturing()` returns `false`.

## cap.ctrl.info.test.start: Capturing is started after being stopped

**References**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 

After capturing is started again, `is_capturing()` returns `true`.
