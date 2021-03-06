# null
Null all of the things! This package was originally created as a joke, but hey now it actually does something non-trivial.

If you ever use `null` for logic tests, you can try using a `Symbol` instead via the NullRef library provided by this package.

This package provides for a `NULL` constant that is a Symbol from the Global Symbol Registry, as well as convenience methods for testing, casting, and comparing values.

## Usage

Require and reference what you need:

```javascript
const nullref   = require('null'); // note that the variable name should not be null, here we use nullref
const nulltest  = nullref.lib; // load the full library of convenience features

const isNull    = nullref.isNull // or just load the main ones you want (checks for null or NULL)
const isNullRef = nullref.isNullRef // checks for NULL only

const NULL = nullref(); // NULL symbol instance (singleton);
```

Consume and use as needed.

```javascript
let x = null;

//returns true is x is null or NULL
if( nulltest.is(x) ) //do something

if( isNull(x) ) // same as above

//cast a variable to NULL if it is null or NULL
if( NULL === nulltest.to(x) ) // do something

```

