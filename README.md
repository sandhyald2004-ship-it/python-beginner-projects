def calculate(number1: float, number2: float, operator: str) -> float:
    """Perform a basic arithmetic operation."""

    if operator == "+":
        return number1 + number2
    if operator == "-":
        return number1 - number2
    if operator == "*":
        return number1 * number2
    if operator == "/":
        if number2 == 0:
            raise ValueError("Division by zero is not allowed.")
        return number1 / number2

    raise ValueError("Unsupported operator.")


def main() -> None:
    try:
        first_number = float(input("Enter the first number: "))
        operator = input("Enter an operator (+, -, *, /): ").strip()
        second_number = float(input("Enter the second number: "))

        result = calculate(first_number, second_number, operator)
        print(f"Result: {result}")

    except ValueError as error:
        print(f"Error: {error}")


if __name__ == "__main__":
    main()# python-beginner-projects
A collection of beginner-friendly Python programs and mini projects.
