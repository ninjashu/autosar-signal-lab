# AUTOSAR Signal Lab

An interactive, single-page teaching simulator for Classic and Adaptive AUTOSAR concepts. Open `index.html` in a browser; there is nothing to build or install.

## Levels

| Platform | Level | What it shows |
|---|---|---|
| Classic | Layer map | Each module's job and typical calls |
| Classic | Signal path | A signal travelling SWC → RTE → COM → PduR → CanIf → Can across CAN, with timeouts and bus faults |
| Classic | OS scheduling | Fixed-priority tasks, preemption, missed deadlines, lost activations |
| Classic | Diagnostics | UDS requests, sessions, security access, fault debouncing into a stored DTC |
| Adaptive | Platform map | Each functional cluster's job |
| Adaptive | Services | Service discovery, event subscription, method calls, link loss |
| Adaptive | Execution and health | Function group state changes, dependency-ordered start and stop, alive supervision and recovery |

Every simulated level records its run, so you can pause, scrub back, replay, and resume from an earlier point. Settings can be changed three ways: controls, an editable JSON config, and an API console.

## Limits

This is a teaching model, not an AUTOSAR stack. Call names and behaviour follow the standard, but there is no generated code, no ARXML and no real timing. Module delays are stretched so they are visible, the seed and key algorithm is a toy, and service discovery is shortened.
