# Bash Scripting Reference Doc

## Basics
#### Initialize and assign variables
```
variable = "string value"
variableInt = 69
variableBool = true
```
#### Access value of a variable
```$variable```
#### Cast value to string
```"$variable"```
#### List of Operators
-eq (equal to)
-ne (not equal to)
-lt (less than)
-gt (greater than)
-le (less than or equal to)
-ge (greater than or equal to)

## Conditionals

## Looping
#### For loop
```
for item in array
do
    echo "instructions go here"
done
```
#### C-style For loop
```
for (( i=0;i<=5;i++ ))
do
    echo "instructions go here"
done
```
#### While loop
```
while [ $variable -eq 3 ]
do
    echo "instructions go here"
done
```
