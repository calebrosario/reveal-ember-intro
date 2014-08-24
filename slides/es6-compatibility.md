##  ES6 Compatibility

```
import $ from "jquery";                    // import the default export of a module
module crypto from "crypto";               // binding an external module to a variable
import { encrypt, decrypt } from "crypto"; // binding a module's exports to variables
import { encrypt as enc } from "crypto";   // binding and renaming one of a module's exports
export * from "crypto";                    // re-exporting another module's exports
export { foo, bar } from "crypto";         // re-exporting specified exports from another module


```

Standard Draft : http://wiki.ecmascript.org/doku.php?id=harmony:specification_drafts
