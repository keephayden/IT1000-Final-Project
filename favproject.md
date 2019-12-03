# Favorite Project I Have Done with Coding
When I started coding this year I was very intimidated because I was going into it blindfolded. I had never learned how to do anything that I was about to be doing for the rest of my life.

---
So, this project was the first project that I had done that felt challenging, but was easy enough to understand how to complete. The point of it was to calculate an objects final position with the variables of acceleration, velocity, time, and initial position.

``` Python
# Object Position Calculation

print("This program calculates an object's final position.\n")

#Get input from the user
do_calculation = True
while (do_calculation):

while (True):
       try:
               initial_position = float(input("Enter the object's initial position: "))
               if (initial_position < 0):
                       print("Negative initial positions are not allowed.")
                       continue
       except ValueError:
                       print("The value you entered is invalid. Only numerical values are valid.")
       else:
                       break
while (True):
       try:
               initial_velocity = float(input("Enter the object's initial velocity: "))
               if (initial_velocity < 0):
                       print("Negative initial velocities are not allowed.")
                       continue
       except ValueError:
                       print("The value you entered is invalid. Only numerical values are valid.")
       else:
                       break
while (True):
       try:
               acceleration = float(input("Enter the object's acceleration: "))
               if (acceleration < 0):
                       print("Negative accelerations are not allowed.")
                       continue
       except ValueError:
                       print("The value you entered is invalid. Only numerical values are valid.")
       else:
                       break
while (True):
       try:
               time_elapsed = float(input("Enter the time that has elapsed: "))
               if (time_elapsed < 0):
                       print("Negative times are not allowed.")
                       continue
       except ValueError:
                       print("The value you entered is invalid. Only numerical values are valid.")
       else:
                       break

# Find the final position

final_position = initial_position + initial_velocity * time_elapsed + 0.5 * acceleration  * time_elapsed ** 2

# Output final position

print("\nThe object's final position is", final_position)

#Ask user to do another calculation

another_calculation = input("Do you want to perform another calculation? (y/n): ")
if (another_calculation != "y"):
       do_calculation = False
```

[Home](./README.md)
