# Task 2 — Formalize Constraints

| Constraint ID | Constraint                                                 | Formal Expression                       | Meaning                                                                    |
| ------------- | ---------------------------------------------------------- | --------------------------------------- | -------------------------------------------------------------------------- |
| C1            | The barrier must not open while a train is present.        | `Train_Present → ¬Barrier_Open`         | If a train is present, the barrier must not be open.                       |
| C2            | The barrier must close when a train approaches.            | `Train_Approaching → Barrier_Closed`    | If a train is approaching, the barrier must be closed.                     |
| C3            | Warning lights must activate when a train approaches.      | `Train_Approaching → Warning_Light_On`  | If a train is approaching, the warning light must be ON.                   |
| C4            | Audible alarm must activate when a train approaches.       | `Train_Approaching → Audible_Alarm_On`  | If a train is approaching, the audible alarm must be ON.                   |
| C5            | Barrier must remain closed while train is passing.         | `Train_Passing → Barrier_Closed`        | While the train is passing, the barrier must remain closed.                |
| C6            | Barrier must not open before train clearance is confirmed. | `¬Train_Cleared → ¬Barrier_Open`        | If the train has not been confirmed as cleared, the barrier must not open. |
| C7            | Sensor failure must not cause unsafe barrier opening.      | `Sensor_Failure → ¬Unsafe_Barrier_Open` | If a sensor fails, an unsafe barrier opening must not occur.               |
| C8            | Barrier failure must activate a safety warning.            | `Barrier_Failure → Safety_Warning_On`   | If the barrier fails, the safety warning must be activated.                |
