for i in {1..10}
do
    echo "Best School"
done: Write a Bash script that displays Best School 10 times

count=1  # Initialize a counter

while [ $count -le 10 ]  # Continue until the counter is greater than 10
do
    echo "Best School"  # Display the message
    ((count++))  # Increment the counter
done: a Bash script that displays Best School 10 times using while loop

#!/usr/bin/env bash
# This script displays 'Best School' 10 times and 'Hi' on the 9th iteration

count=1  # Initialize a counter

while [ $count -le 10 ]  # Continue until the counter is greater than 10
do
    if [ $count -eq 9 ]; then  # Check if the counter is 9
        echo "Best School"  # Display the message
        echo "Hi"  # Display 'Hi' on a new line
    else
        echo "Best School"  # Display the message
    fi
    ((count++))  # Increment the counter
done: a Bash script that displays Best School 10 times, but for the 9th iteration, displays Best School and then Hi on a new line
