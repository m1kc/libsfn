libsfn reference
================

Connect and disconnect
----------------------

Methods:
  Listening specified port.
  Connect to specifies host and port.
  Disconnect.
  
Listeners:
  Connection established listener.
  Disconnect listener.


Capabilities
------------

Obtain remote client name, version.


Send files
----------

Methods:
  Append files to queue (array of: file name, file size, MD5)
  Remove files from queue  (array of: file name, MD5)
  Accept file request (file name, MD5)

Listeners:
  Append files listener (array of: file name, file size, MD5)
  Remove files listener (array of: file name, MD5)
  Accept file listener (file name, MD5, boolean Accept/Deny - may be, no such space)


Send messages and other optional stuff
--------------------------------------

Methods:
  Request local free space.
  Request remote free space.
  Send message.
  
Listeners:
  Incoming message listener.
