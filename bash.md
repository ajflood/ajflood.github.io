Necessary Header: #!/bin/bash

Creating a function: 
```bash
function theName {
          #Echo first argument
          echo $1} ```
          
Checking if arguments exist:
```
if [ ! -z $1 ] 
then 
    : # $1 was given
else
    : # $1 was not given
fi
```

Capturing arguments:  
`args="$@"`
