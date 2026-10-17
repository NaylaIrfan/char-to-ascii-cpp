# char-to-ascii-cpp

# ASCII Value of Each Character (C++)

A beginner-friendly C++ program that finds and prints the ASCII value of each character in a string entered by the user.

## About

Every character is stored in a computer as a number, called its **ASCII value**. This program reads a line of text and prints each character along with its ASCII value, including spaces, digits and symbols.

## Example

```
Enter a string: Hi 5
Character -> ASCII value
   H      ->  72
   i      ->  105
          ->  32
   5      ->  53
```

## Useful ASCII Values

| Characters | ASCII range |
|------------|-------------|
| `0` to `9` | 48 to 57 |
| `A` to `Z` | 65 to 90 |
| `a` to `z` | 97 to 122 |
| Space | 32 |

## How It Works

1. Read the full line using `getline(cin, str)`.
2. Go through each character one by one using a `for` loop.
3. Print the character using `str[i]`.
4. Convert the character to an integer using `(int)str[i]` and print it. This gives the ASCII value.

## Single Character Version

To find the ASCII value of just one character, read it into a `char` variable and print `(int)ch`:

```cpp
char ch;
cin >> ch;
cout << (int)ch;
```

## Things to Note

- `(int)` is called **type casting**. It converts a `char` into its numeric value.
- Without the cast, `cout` would print the character itself and not its number.
- The difference between a small letter and its capital letter is always 32 (for example, `'a'` is 97 and `'A'` is 65).

## Concepts Used

- Strings (`string`)
- `char` and `int` data types
- Type casting
- Input and output (`cin`, `cout`, `getline`)
- `for` loop
- String indexing (`str[i]`)

## How to Run

Make sure a C++ compiler such as `g++` is installed.

```bash
# Compile
g++ ascii_value.cpp -o ascii_value

# Run (Linux / macOS)
./ascii_value

# Run (Windows)
ascii_value.exe
```

## Project Structure

```
ascii-value-cpp/
├── README.md
└── ascii_value.cpp
```

## Author

NAYLA IRFAN
B.Tech CSE

## License

This project is free to use for learning purposes.
