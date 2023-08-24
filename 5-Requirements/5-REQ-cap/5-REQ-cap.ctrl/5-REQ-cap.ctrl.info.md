# cap.ctrl.info: Get Capturing-State

**References:**

- in branch [main](https://github.com/mhatzl/evident/tree/main): 1 (1 direct)

As a user, I want to know if capturing is active or not, because I want to stay informed about the capturing state.

## cap.ctrl.info.test.init: Capturing is active initially

Capturing is active initially: `is_capturing()` returns `true`.

## cap.ctrl.info.test.stop: Capturing is stopped

After capturing is stopped, `is_capturing()` returns `false`.

## cap.ctrl.info.test.start: Capturing is started after being stopped

After capturing is started again, `is_capturing()` returns `true`.
