Qt Blocking Queue
=================

The fork was created to extend the functionality of original project by Qize Huang.

Additions and changes:
=================
1. The "bool get(T* val, unsigned long msec)" method has been added to the "BlockQueue" class to allow setting the waiting time for an element in the queue (rather than infinite waiting, as in the usual "get" method);
2. In the "Event" class, the "set" method no longer checks if the flag is already set, because (for unknown reasons) sometimes threads would not wake up the first time the flag was set, and the check would prevent them from being woken up on subsequent calls to this method.


License
=======

Same as original project.



