Patch json for firebase update calls

## Features

* Patching
* Diffing

## Usage

```dart
import 'package:json_patch/json_patch.dart';

var from = {
  "key": "value",
  "key2": {
    "key3": "value3"
  }
};

var into = {
  "key": "anotherValue",
  "key2": {
    "key3": "value3"
  }
};

var patch = from.diff(into);
var updated = from.patched(patch); // returns same contents as 'to'
```