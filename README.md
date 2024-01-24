# OpenAICostCalculator

## Overview
`OpenAICostCalculator` is a Python tool designed to calculate the cost of using OpenAI's API in various scenarios, particularly focusing on applications like the "Doctor Diagnosis Assistant App". It takes into account the number of prompts, the average number of tokens per prompt, the cost per token, and other relevant factors to provide a comprehensive cost analysis.

## Features
- Calculate the cost of using OpenAI's API per shift, per day, per month, and annually.
- Customizable inputs for different scenarios.
- Outputs a clear and detailed cost breakdown.
- Descriptive scenario summary based on user inputs.

## Installation

Clone the repository:
```bash
git clone https://github.com/mrodgers/example_token_use.git
cd OpenAICostCalculator
```

Ensure you have Python installed. This project requires Python 3.6 or later. You can download Python from [here](https://www.python.org/downloads/).

## Usage

Run the script in the command line:

```bash
python token_calc.py
```

Follow the on-screen prompts to enter the required information:
- Number of prompts per doctor's shift.
- Chain/Interaction/Augmentation multiplier.
- Average tokens used per API call.
- OpenAI cost per 1000 tokens.
- Number of doctors on shift per hospital.
- Number of shifts per day.

## Example

```python
# Initialize the calculator with example values
calculator = OpenAICostCalculator(50, 2, 4000, 0.045)

# Calculate and display the costs
cost_per_shift = calculator.calculate_cost_per_shift()
print(f"Cost per shift: ${cost_per_shift:.2f}")
```

## Contributing

Contributions to `OpenAICostCalculator` are welcome! Here are ways you can contribute:
- Submitting bug reports and feature requests.
- Writing code for new features or bug fixes.
- Improving documentation.

## License

This project is licensed under the [MIT License](LICENSE.md).

## Disclaimer

This tool is provided as-is, and it is not officially associated with OpenAI. Please use it responsibly and in accordance with OpenAI's pricing policy.

---

Developed with ❤ by Matt Rodgers
