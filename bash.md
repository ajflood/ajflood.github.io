Necessary Header: #!/bin/bash

Creating a function: 
```bash
function theName {
          #Echo first argument
          echo $1} ```
          
if then syntax
```
if TEST-COMMANDS; then
	CONSEQUENT-COMMANDS;
elif MORE-TEST-COMMANDS; then
	MORE-CONSEQUENT-COMMANDS;
else 
	ALTERNATE-CONSEQUENT-COMMANDS;
fi
```

Checking if arguments exist:
```
if [ ! -z $1 ]; then 
    : # $1 was given
else
    : # $1 was not given
fi
```

Capturing arguments:  
`args="$@"`
