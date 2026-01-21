# Aegis

A secure messaging application built with SwiftUI, implementing advanced cryptographic protocols for end-to-end encrypted communication. Aegis focuses on privacy and security with features like zero plaintext in memory, encrypted storage, and secure UI measures.

## Features

- **End-to-End Encryption**: Implementation of the Double Ratchet algorithm for forward secrecy and deniability
- **Message Layer Security (MLS)**: For secure group messaging with Post-Compromise Security
- **Secure Enclave Integration**: Hardware-backed identity and key management
- **Encrypted Storage**: SQLCipher for secure data persistence with monotonic versioning in Keychain
- **Onion Routing**: For enhanced privacy in message routing
- **Secure UI**: Automatically blurs screenshots and prevents sensitive data exposure
- **Key Security**: Replay detection, rollback prevention, and automatic key zeroization
- **VCard Support**: For contact sharing with encryption

## Security Measures

- Zero plaintext data in memory
- Encrypted database storage
- Hardware security integration
- Debugger resistance
- Automatic key wipe on failures
- Privacy-sensitive UI elements

## Technologies Used

- SwiftUI for the user interface
- CryptoKit for cryptographic primitives
- GRDB with SQLCipher for encrypted database
- Secure Enclave for hardware-backed keys
- Custom implementations of Double Ratchet, MLS, and onion routing

## Installation

1. Clone the repository:
   ```
   git clone <https://github.com/Traianosv/Aegis>
   cd Aegis
   ```

2. Open the project in Xcode:
   ```
   open Aegis.xcodeproj
   ```

3. Build and run the project using Xcode.

## Requirements

- macOS (or iOS, depending on target)
- Xcode 15.0 or later
- Swift 5.9 or later

## Architecture

The project is organized into several key components:

- **Core**: Cryptographic primitives, MLS implementation, message handling
- **UI**: SwiftUI views for messaging, conversations, onboarding
- **Storage**: Encrypted database and secure state persistence
- **Networking**: Onion routing and relay client
- **Utils**: Secure buffers and extensions

## Contributing

Please ensure all contributions maintain the security-first principles of Aegis. Run tests before submitting changes.

## License

MIT

