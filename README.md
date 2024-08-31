# Genetic Algorithm for Intrusion Detection System Configuration

This repository contains the implementation of a Genetic Algorithm designed to optimize the configuration of an Intrusion Detection System (IDS). The algorithm aims to find the best ruleset for each IDS to maximize the detection of attack steps while minimizing false positives and undetected attacks.

## Features

- **Sparse Matrix Generation**: Generates sparse random matrices to simulate attack paths, IDS to attack step relationships, and rule requirements.
- **Initial Population Generator**: Randomly generates an initial population of IDS configurations.
- **Fitness Function**: Evaluates each configuration based on detection effectiveness, false positives, and the cost of undetected attacks.
- **Genetic Algorithm Implementation**: Utilizes the `pygad` library for evolving solutions through selection, crossover, and mutation.
- **Custom Stopping Criteria**: Implements a custom stopping condition based on the average detection performance.

## Installation

1. **Clone the repository**:  
   git clone https://github.com/yourusername/genetic-algorithm-ids.git

2. **Install the required Python packages**:  
   pip install numpy pygad

## Usage

1. **Configure Parameters**: Modify the parameters such as the number of IDS, rules, attack steps, and paths in the script as per your requirement.

2. **Run the Algorithm**: Execute the script to start the Genetic Algorithm.  
   python main.py

3. **View Results**: The best solution and its fitness value will be printed in the console.

## Example

An example of how to set up and run the Genetic Algorithm is provided in the `example.py` file.

## Customization

- **Matrices and Parameters**: You can adjust the sparsity of matrices, number of attack paths, IDS, and rules to simulate different scenarios.
- **Fitness Function**: Customize the fitness function to emphasize different aspects such as false positives or undetected attacks.
- **Stopping Criteria**: Adjust the custom stopping criteria to suit your performance requirements.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an Issue for suggestions and improvements.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

Special thanks to the `pygad` library contributors for providing a robust Genetic Algorithm framework.
