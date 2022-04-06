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
#### if then else
```
if [ $variable -le 5 ]
then
    echo "instructions go here"
else
    echo "more instructions"
fi
```

## Looping
#### For loop
```
for item in someList
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
#### For loop with range
For a range with default step of 1:
```
for value in {1..5}
do
    echo $value
done
```
For a range with custom step:
```
for value in {0..10..2}
do
    echo $value
done
```
Negative step is automatically applied:
```
for value in {10..0..2}
do
    echo $value
done
```
#### While loop
```
while [ $variable -eq 3 ]
do
    echo "instructions go here"
done
```
