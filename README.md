# MiniShell Variable Expansion Tester

[![42 School](https://img.shields.io/badge/42-School-blue)](https://42firenze.it/)
[![GitHub license](https://img.shields.io/github/license/Nazar963/Tester_variable_expansion)](https://github.com/Nazar963/Tester_variable_expansion/blob/master/LICENSE)

A comprehensive testing suite for the variable expansion functionality in the 42 School MiniShell project.

## 📋 Overview

This project provides an automated testing framework specifically designed to test the variable expansion capabilities of your MiniShell implementation. It systematically checks how your shell handles environment variables in different contexts, including:

- Variables within different types of quotes (single, double)
- Multiple variables in sequence
- Variables with different combinations of quotes
- Edge cases and complex scenarios

## 🚀 Features

- 100+ comprehensive test cases
- Automated testing with clear pass/fail indicators
- Detailed comparison between expected and actual outputs
- Easy to run and integrate into your development workflow

## 🛠️ Prerequisites

- A Unix-like operating system (Linux/macOS)
- Bash shell
- GCC compiler and Make
- Your MiniShell project with a Makefile in the parent directory

## 📂 Project Structure

```
Tester_variable_expansion/
├── .vscode/
│   └── mcp.json            # Model Context Protocol configuration
├── tester/
│   ├── expected_outputs.txt # Expected output from a correct implementation
│   ├── inputs.txt           # Test commands to run
│   ├── outputs.txt          # Results from your implementation (generated)
│   └── test_script.sh       # Testing script
└── README.md               # This file
```

## 📥 Installation

1. Clone your MiniShell project into a directory
2. Clone this repository next to your MiniShell directory:

```bash
git clone https://github.com/yourusername/Tester_variable_expansion.git
```

## 🧪 Running the Tests

1. Make sure your MiniShell project is in the correct relative path as expected by the tester
2. Navigate to the tester directory:

```bash
cd Tester_variable_expansion/tester
```

3. Run the test script:

```bash
./test_script.sh
```

The script will:
- Compile your MiniShell project using its Makefile
- Run each test case and capture the output
- Compare the output with expected results
- Display any differences found

## 📊 Test Cases

The test cases focus on variable expansion in different contexts:

1. Basic variable expansion (`$USER`)
2. Variables within double quotes (`"$USER"`)
3. Variables within single quotes (`'$USER'`) - which should not expand
4. Complex combinations (`$USER '$USER' "$USER"`)
5. Multiple variables (`$USER $USER $USER`)
6. Variables with adjacent text
7. Nested quotes (`"'$USER'"`)
8. And many more edge cases!

## 🔍 Understanding Test Results

When running the tests, for each failed test, you will see:
- The test number
- The actual differences between expected and received outputs
- Side-by-side comparison to easily spot discrepancies

A successful test run will not show any failures.

## ⚙️ Customization

You can modify the testing framework for your needs:

- Edit `test_script.sh` to change testing parameters
- Add new test cases to `inputs.txt` and corresponding expected outputs to `expected_outputs.txt`
- Update the path to your MiniShell executable in `test_script.sh`

## 📝 Test Coverage

The tester covers the following aspects of variable expansion:

- Environment variable substitution
- Handling of variables in different quote contexts
- Multiple variable occurrences
- Edge cases and special characters
- Behavior with empty or non-existent variables

## 🤝 Contributing

Feel free to submit issues or pull requests if you have suggestions for improving the test suite or adding more test cases.

## 📜 License

This project is open source and available under the [MIT License](LICENSE).

## 🔗 Related Projects

- [42 School MiniShell Project](https://github.com/Nazar963/42_minishell)

## 📧 Contact

For questions or feedback, please open an issue in the repository.

⭐ **Star this repository if you found it helpful!**  
[![GitHub stars](https://img.shields.io/github/stars/Nazar963/Tester_variable_expansion?style=social)](https://github.com/Nazar963/Tester_variable_expansion/stargazers)

[![42 School](https://img.shields.io/badge/42-profile-blue)](https://profile-v3.intra.42.fr/users/naal-jen)
[![GitHub Profile](https://img.shields.io/badge/GitHub-Nazar963-lightgrey)](https://github.com/Nazar963)
---

Good luck with your MiniShell project at 42! 🚀
