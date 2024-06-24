# Rosario's Enigma Encryption Tool

## Description

Rosario's Enigma Encryption Tool is a secure password management system inspired by the concept of the Enigma machine. It provides a unique, interactive way to set up and validate passwords using a color-coded grid system and directional inputs.

![Rosario's Enigma](https://github.com/DylanCkawalec/ros-enigma/assets/43707795/67b37056-834a-43c0-8378-e9b4f3c5562d)

## Features

- Secure password encryption using `AES-256-GCM`
- Interactive color-symbol and direction-symbol mapping setup
- Visual grid-based password validation
- Strong password encouragement with `zxcvbn` password strength estimation
- Configuration persistence

## Installation

1. Ensure you have Rust installed on your system. If not, install it from [https://www.rust-lang.org/](https://www.rust-lang.org/).

2. Clone this repository:
   ```
   git clone https://github.com/your-username/rosarios-enigma-encryption-tool.git
   ```

3. Navigate to the project directory:
   ```
   cd rosarios-enigma-encryption-tool
   ```

4. Build the project:
   ```
   cargo build --release
   ```

5. Run the program:
   ```
   cargo run --release
   ```

## How to Use

1. **Initial Setup**: On first run, the program will guide you through setting up your personalized configuration:
   - Assign symbols to colors
   - Assign symbols to directions
   - Create a secure password

2. **Main Menu**: After setup, you'll see the main menu with these options:
   1. Generate new grid and validate password
   2. View current configuration
   3. Reset configuration
   4. Exit

3. **Password Validation**:
   - A color-coded grid will be displayed
   - Use arrow keys to select the direction corresponding to your password character
   - Repeat for each character in your password

## How It Works

1. **Password Encryption**: Your password is encrypted using AES-256-GCM and stored securely.

2. **Color-Symbol Mapping**: You assign symbols (♦, ♥, ♠, ♣) to colors (Red, Green, Blue, Yellow).

3. **Direction-Symbol Mapping**: You assign the same symbols to directions (Left, Up, Right, Down).

4. **Grid Generation**: When validating, a grid is generated with your password characters hidden among random characters.

5. **Validation Process**: 
   - Each password character is placed in a specific color zone.
   - You input the direction corresponding to the symbol assigned to that color.
   - The program checks if your input matches the expected character.

6. **Security**: The system never directly compares your input to the raw password, adding an extra layer of security.

## Security Considerations

- The program uses strong encryption (AES-256-GCM) to store your password.
- The visual nature of the validation process helps protect against keyloggers.
- The password is never stored in plain text.

## Contributing

Contributions, issues, and feature requests are welcome. Feel free to check [issues page](https://github.com/your-username/rosarios-enigma-encryption-tool/issues) if you want to contribute.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
This project IS NOT Licensed for any purposes other than being purely educational. The Rosario Enigma Proof is a patented technology and should be considered for public domain applications because of it's ability to provide zero-knowledge proofs to hardware wallet applications, KSM's, Trusted Enclave telecomunication services and digital social recovery services.