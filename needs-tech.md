# Visit-counter technical needs

## Scenario: Recover across restarts of the server that runs the visit-counter

- Given:Sensor is working accurately.
- When: Sensor needs a restart.
- Then: Get the last visitor count before the system gets restart.
        And start incrementing the visitor count from there.

## Scenario: Reconcile counts if the sensor is offline for a while

- Given : Sensor is offline for sometime.
- When: During visitors are visiting.
- Then: Store the count of visitor before the sensor is offline.
          Store the count of visitor after the sensor is offline.
          And predict the count of visitor during this sensor offline time.
          And show the sum of all three counts.
