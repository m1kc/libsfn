libsfn reference
================

Connect and disconnect
----------------------

### Methods:
* Listening specified port.
* Connect to specified host and port.
* Disconnect.
  
### Listeners:
* Connection established listener. Tells remote address.
* Disconnect listener.


Capabilities
------------

* Obtain remote client name, version.


Send files
----------

### Methods:
* Append files to queue (array of: file name, file size, MD5) `зачем массив?`
* Remove files from queue  (array of: file name, MD5)
* Accept file request (file name, MD5)

`а зачем нам вообще подтвеpждение пеpедачи?`
`если я запустил пpогpамму и установил с тобой соединение - вpяд ли я в последний момент пеpедумаю`

### Listeners:
* Append files listener (array of: file name, file size, MD5)
* Remove files listener (array of: file name, MD5)
* Accept file listener (file name, MD5, boolean Accept/Deny - may be, no such space)
* Transfer status (file name, MD5, processed bytes, rate)


Send messages and other optional stuff
--------------------------------------

### Methods:
* Request local free space. `с какой ФС?`
* Request remote free space. `с какой ФС?`
* Send message.
  
### Listeners:
* Incoming message listener.
