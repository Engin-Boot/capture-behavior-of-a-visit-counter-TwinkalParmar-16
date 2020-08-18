# Visit-counter technical needs

## Scenario: Recover across restarts of the server that runs the visit-counter

  - Given
  - When
  - Then

## Scenario: Reconcile counts if the sensor is offline for a while

  - Given : Sensor is offline for sometime.
  - When: During visitors are visiting.
  - Then: Store the count of visitor before the system failure or sensor is offline.
          Store the count of visitor after the system failure or sensor is offline.
          And predict the count of visitor during this failure.
          And finally show the sum of all three counts.
