# Temperature_Conversion
# This is my First Python Code to convert Celsius to Fahrenheit

def celsius_to_fahrenheit(celsius):
    try:
        fahrenheit = (celsius * 9/5) + 32
        return fahrenheit
    except TypeError:
        raise ValueError("Invalid input! Please provide a valid temperature in Celsius.")

# Example usage
celsius = input("Enter the temperature in Celsius: ")

try:
    celsius = float(celsius)
    fahrenheit = celsius_to_fahrenheit(celsius)
    print(f"{celsius} degrees Celsius is equal to {fahrenheit} degrees Fahrenheit.")
except ValueError as e:
    print(str(e))
