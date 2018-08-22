Necessary Header: #!/bin/bash

Creating a function: 
```bash
function theName {
          #Echo first argument
          echo $1}
```

Create Array:
```bash 
some_array=(value1 value2 ... valueN)
```

Loop over array:
```bash
for i in "${arr[@]}"
do
   echo "$i"
done
```

For i in sequence:
```bash
for i in {1..5}
do
    echo "Welcome $i times"
done
```

if then syntax
```bash
if TEST-COMMANDS; then
	CONSEQUENT-COMMANDS;
elif MORE-TEST-COMMANDS; then
	MORE-CONSEQUENT-COMMANDS;
else 
	ALTERNATE-CONSEQUENT-COMMANDS;
fi
```

Checking if arguments exist:
```bash
if [ ! -z $1 ]; then 
    : # $1 was given
else
    : # $1 was not given
fi
```

Capturing arguments:  
`args="$@"`
