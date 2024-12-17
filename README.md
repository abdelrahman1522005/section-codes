# section-codes
# section 1 : Docstring
def divide(a, b):
    """
    Divide two numbers.
       Args:
         a (float): The numerator.
         b (float): The denominator.

  Returns:
       float: The result of division.

   Raises:
        ZeroDivisionError: If the denominator is zero.
    """
  if b == 0:
      raise ZeroDivisionError("Denominator cannot be zero")
    return a / b

# 1. PEP 257
# Python's official guidelines for writing docstrings:

# Use triple quotes for all docstrings.
# The first line should be a short summary of the object’s purpose.
# Add a blank line after the summary if additional explanation is included.
# Keep line length within 72 characters for compatibility
# 2. Google Style
# A widely adopted format for detailed docstrings.

def multiply(a, b):
    """
    Multiply two numbers.

    Args:
        a (int): The first number.
        b (int): The second number.

    Returns:
        int: The product of the two numbers.
    """
  return a * b
    
    
# 3. NumPy Style
# Popular in scientific computing and data analysis.

def square_root(x):
    """
    Compute the square root of a number.

    Parameters
    ----------
    x : float
        The number to find the square root of.

    Returns
    -------
    float
        The square root of the number.
    """
    return x ** 0.5
    
    
# Accessing Docstrings
# Docstrings are stored in the __doc__ attribute of the object.

def greet(name):
    """Greet a person by their name."""
    return f"Hello, {name}!"

print(greet.__doc__)  # Output: Greet a person by their name.

 
