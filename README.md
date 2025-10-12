# ESQL Language Support

This is the README for your extension "org-github-vscode-extendedsql-language". After writing up a brief description, we recommend including the following sections.

## Features

This extension provides the following features for ESQL files:

- **Syntax Highlighting**: Full syntax highlighting for ESQL keywords, functions, operators, strings, and comments
- **Language Configuration**: Proper bracket matching, auto-closing pairs, and comment support
- **File Association**: Automatic detection of `.esql` files
- **Code Formatting**: Proper indentation and formatting support

### Supported ESQL Features

- **Commands**: FROM, WHERE, EVAL, STATS, SORT, LIMIT, KEEP, DROP, RENAME, DISSECT, GROK, ENRICH, LOOKUP, MV_EXPAND, ROW
- **Operators**: Comparison (==, !=, <, >, <=, >=), Arithmetic (+, -, *, /, %), Logical (AND, OR, NOT)
- **Functions**: Mathematical, String manipulation, Date/time, Statistical aggregations, Multi-value functions, and more
- **Data Types**: Numbers, strings (single, double, backtick quoted), booleans, null values
- **Comments**: Line comments (//) and block comments (/* */)

## Requirements

- Visual Studio Code 1.105.0 or higher

## Usage

1. Open any file with the `.esql` extension
2. The extension will automatically provide syntax highlighting and language features
3. Create new ESQL files and start writing queries with full language support

### Example ESQL Query

```esql
FROM employees
| WHERE department == "Engineering"
| EVAL bonus = salary * 0.1
| STATS avg_salary = AVG(salary), total_bonus = SUM(bonus) BY department
| SORT avg_salary DESC
```

## Installation

1. Open Visual Studio Code
2. Go to the Extensions view (Ctrl+Shift+X)
3. Search for "ESQL Language Support"
4. Click Install

## Contributing

This extension is open source. Contributions are welcome!

## Release Notes

### 0.0.1

Initial release of ESQL Language Support:
- Basic syntax highlighting for ESQL
- Language configuration for brackets and comments
- File association for .esql files

## License

MIT License

---

**Enjoy writing ESQL queries with enhanced language support!**
