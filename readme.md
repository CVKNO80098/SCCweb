# SCC - Secure Content Cryptographer

SCC (Secure Content Cryptographer) is a command-line encryption program that allows you to encrypt and decrypt text using a password. It provides a simple and secure way to protect your sensitive information.

## Usage

```cmd
SCC -L <str> -p <password> | -U <str> -p <password> |-w <address> [--version] [--help]
```


## Options

- `-L <str>`: Specifies the text to encrypt with the given password (`<str>` represents the text).
- `-p <password>`: Specifies the password (`<password>` represents the password).
- `-U <str>`: Specifies the text to decrypt with the given password (`<str>` represents the text).
- `-w <address>`: Enables output to be saved as a txt file. The optional `<address>` specifies the file path. If no address is provided, it defaults to "temp.txt".
- `--version`: Displays the program version information.
- `--help`: Displays the help information.

Please note that the `-w` option must be specified last and can be left empty.

## Examples

- Encrypting text:

```
SCC -L "Hello, World!" -p MyPassword -w output.txt
```

- Decrypting text:

```
SCC -U "encrypted_text" -p MyPassword
```
- Saving encrypted/decrypted text to a file (default path: temp.txt):
```
SCC -L "Hello, World!" -p MyPassword -w
```
- Displaying program version:
```
SCC --version
```
- Displaying help information:
```
SCC --help
```

## License

This project is licensed under the GNU License. See the [LICENSE](./Contact.html) file for details.
