# Password Generator

A simple Python script I built to generate strong passwords from the command line. It mixes uppercase, lowercase, numbers and symbols — and yells at you in red if you enter something wrong.

## How to Run
```bash
python main.py
```

## Requirements
- Python 3.x

## How it Works
1. Enter your desired password length (minimum 8)
2. The script validates your input
3. Generates a randomized strong password instantly

## Example
```
How long you want your password to be? (atleast 8) : 12
Strong Password: aB3#kP9@mX2!
```

## What I Used
- Python 3
- `string` and `random` modules
- ANSI color codes for terminal output