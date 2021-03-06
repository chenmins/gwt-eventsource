## 1.0:

* Minor documentation improvements.

## 0.6:

* Improve the javadocs.
* Move EventSource to using EventSourceListener interface as the primary means of notifying library
  consumers of EventSource events. Add an EventBasedEventSourceListener to support the previous
  event-oriented mechanisms of integrating with the EventSource library.

## 0.5:

* Support subscription from and to multiple event types via subscribeTo and unsubscribeFrom methods
  on EventSource.

## 0.4:

* Add getLastEventId() and getMessageType() methods to MessageEvent to expose underlying message
  characteristics.
* Ensure EventSource.getReadyState() will always return a non null value (CLOSED if not connected).
* Support a variant of EventSource.open() that sets withCredentials option.
* Rename EventSource.connect() to EventSource.open() to match terminology of underlying construct.
* Add support for EventSource.getURL() and EventSource.getWithCredentials() methods.

## 0.3:

* Restore JDK 6 compatibility.

## 0.2:

* Support EventSource.isSupported() method that will return true if EventSource.newEventSourceIfSupported()
  will not return a null value.

## 0.1:

* Initial release
