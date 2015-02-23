<a name="EventPriorityEmitter"></a>
#EventPriorityEmitter([eventName=], [options])
Public interface for using EventPriorityEmitter.

**Params**

- \[eventName=\] `String` - Name to give to the event.  
- \[options\] `Object` | `function` - An object for options or function to subscribe. Certain options
  - \[pub\] `Object` - For event publishing. If eventName is passed
  - \[rePub\] `Boolean` - If set to true and subscribing to an event and the event had
  - \[unSub\] `String` - Required for un-subscribing from priority list.
  - \[sub\] `function` - Required for subscribing to an event.  
  - \[subId\] `String` - Optional for subscribing. Use for identifying and removing
  - \[priority\] `int` - 0-11 where 0 is the lowest (last subscriber to get published data) priority 
  - \[timing\] `String` - When the priority should happen.

**Returns**: `undefined` | `function` - "new EventPriorityEmitter" returns a function with a new
**Example**  
//subscribe using default config

**Example**  
//subscribe default timing

**Example**  
//subscribe post timing

**Example**  
//publish object with data inside the you want subscribers to consume

**Example**  
//un-subscribe a subId
