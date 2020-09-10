# what-is-not-mdm
There is a lot of potential for overlap.  Noting what is _not_ in MDM can help for planning

### Only send in Create/Update data
MDM cannot just receive a "snapshot" of all current data from a system and process it.  This is because anything fed into MDM gets a unique id (ROWID_OBJECT) so imagine how quickly you will overflow.  You should only feed it what it needs to know, which are Create and Update type of events.  ROWID_OBJECT is CHAR(14) so there is generally plenty of runway.
