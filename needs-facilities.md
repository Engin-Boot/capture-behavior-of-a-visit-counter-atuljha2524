# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given there is an operation of a patient
  When visitors come for that patient
  Then make a report counting visitors for
  the patient

Scenario: Alert when seating capacity is full

  Given there are no seats left
  When new visitor comes near the gate
  Then alert occurs
