try_again = True
while (try_again): 
  operation = int(input("Enter which operation you would like to perform \n1. Addition \n2. Subtraction \n3. Multiplication \n4. Division \n"))
  if operation == 1 or operation == 2 or operation == 3 or operation == 4:
    num1 = int(input("\nEnter the first number: "))
    num2 = int(input("Enter your second number: "))
    if operation == 1:
      print("\nThe 2 values add up to ",num1 + num2, "\n")
    elif operation == 2:
      print("\nThe 2 values subtract to ",num1 - num2, "\n") 
    elif operation == 3:
      print("\nAfter multiplying the values you get ",num1 * num2, "\n")
    else:
      print("\nAfter dividing the values you get ",num1 / num2, "\n")
      
    option = input("\nWould you like to try again? ") 
    if option.lower == "yes":
      print("Okay let's try again") 
      try_again = False 
    else:
      try_again = True 
  else:
    print("\nPlease enter a valid operation\n")
else:
  print("Thank you for using the calculator\n")  
  
