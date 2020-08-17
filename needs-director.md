# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given sensor is working fine and beds are available
  When a patient passes the sensor
  Then Count of patient visits increment by 1

Scenario: Compute parking slots to reserve for visiting specialists

  Given the empty slots are there
  When a specialist is visiting the hospital
  Then reserve the slot for him/her
