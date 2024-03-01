#!/bin/bash

# Get current month and day
month=$(date +%m) # Month (01-12)
day=$(date +%d) # Day of the month (01-31)

# Function to calculate GCD in Bash
gcd() {
    if [ $2 -eq 0 ]; then
        echo $1
    else
        gcd $2 $(($1 % $2))
    fi
}

# Calculate GCD of month and day
gcd_result=$(gcd $month $day)

# Format and print the password
printf "password for today is: %x%02d-%02x%02d\n\n" $month $month $day $gcd_result
