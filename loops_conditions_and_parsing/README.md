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


#!/usr/bin/env bash

# This script processes Apache log files to count occurrences of IP addresses and HTTP status codes

# Define the log file location (update this path as necessary)
LOG_FILE="/path/to/apache/logfile.log"

# Check if the log file exists and is readable
if [[ ! -r "$LOG_FILE" ]]; then
    echo "Error: Log file does not exist or is not readable."
    exit 1
fi

# Process the log file
awk '
    {
        # Check if the line has enough fields
        if (NF < 9) {
            print "Error: Wrong format log file."
            exit
        }
        
        # Group by IP and HTTP status code
        count[$1 " " $9]++
    } 
    END {
        # Print occurrences in the desired format
        for (entry in count) {
            print count[entry], entry
        }
    }
' "$LOG_FILE" | sort -nr || echo "Error: Empty log file."

