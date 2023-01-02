---
title: "Python: relative import"
date: 2023-01-02T10:02:43-08:00
snippets: ['Python']
draft: false 
---

To test relative imports before installing a package, add the source code directory to the path.

For example, import code from a file functions.py in src/mypackage/

```Python
import sys
sys.path.append('/Users/username/project/src/')

import mypackage.functions as f
```

