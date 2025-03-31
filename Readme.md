# pra-decode

`pra-decode` is a simple and efficient JavaScript implementation of the SHA-256 hashing algorithm. It provides a secure way to encode messages into a fixed-length hash.

## Features
- 🔒 **Secure Hashing**: Implements SHA-256 algorithm to ensure data integrity.
- ⚡ **Lightweight**: No external dependencies, making it fast and easy to use.
- 📦 **Easy to Use**: Simple function-based implementation for encoding messages.

## Installation
You can install `pra-decode` via npm:

```sh
npm install pra-decode
```

Or using yarn:

```sh
yarn add pra-decode
```

## Usage
Import the package and use it to hash any string:

```javascript
const pra_decode = require("pra-decode");

const message = "Hello, World!";
const hash = pra_decode(message);

console.log("SHA-256 Hash:", hash);
```

### Example Output
```sh
SHA-256 Hash: a591a6d40bf420404a011733cfb7b190d62c65bf0bcda32b53f190da45306c10
```

## How It Works
The `pra_decode` function implements the SHA-256 hashing algorithm by:
1. Initializing constants based on the SHA-256 specification.
2. Preprocessing the input message by padding it to fit block sizes.
3. Processing the message in 512-bit chunks.
4. Performing bitwise operations and modular additions to compute the final hash.
5. Returning the final hashed output as a hexadecimal string.

## API Reference
### `pra_decode(message: string) -> string`
Hashes the given message using SHA-256 and returns a hex-encoded string.

**Parameters:**
- `message` (string) - The input string to be hashed.

**Returns:**
- A SHA-256 hashed string in hexadecimal format.

## Contributing
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit (`git commit -m "Added new feature"`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

## License
This project is licensed under the MIT License.

## Contact
For any queries or support, reach out to:
- 📧 Email: prashantsharma0512@gmail.com
- 🔗 GitHub: [PrashantSharma0512](https://github.com/PrashantSharma0512/pra-decode)

