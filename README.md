# My-code
def add(num1, num2):
  """Adds two numbers and returns the result."""
  return num1 + num2

def subtract(num1, num2):
  """Subtracts two numbers and returns the result."""
  return num1 - num2

def multiply(num1, num2):
  """Multiplies two numbers and returns the result."""
  return num1 * num2

def divide(num1, num2):
  """Divides two numbers and returns the result, handling division by zero."""
  if num2 == 0:
    return "Error: Cannot divide by zero"
  else:
    return num1 / num2

# Get user input
while True:
  try:
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))
    break
  except ValueError:
    print("Invalid input. Please enter numbers only.")

# Get operation choice
operation = input("Choose operation (+, -, *, /): ")

# Perform calculation based on choice
if operation == "+":
  result = add(num1, num2)
elif operation == "-":
  result = subtract(num1, num2)
elif operation == "*":
  result = multiply(num1, num2)
elif operation == "/":
  result = divide(num1, num2)
else:
  result = "Invalid operation"

# Print the result
print(f"Result: {result}")
