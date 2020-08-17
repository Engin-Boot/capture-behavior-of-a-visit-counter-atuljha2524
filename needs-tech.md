# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given the server is restarting
  When the visitors enter
  Then count this temporary visitors in back up server.

Scenario: Reconcile counts if the sensor is offline for a while

  Given the sensor is offline
  When the visitors enter
  Then don't count them and
  restart from where it left
