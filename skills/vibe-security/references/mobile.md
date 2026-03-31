# Mobile Security

All secrets in the JS bundle are extractable. Use a backend proxy for API calls requiring secret keys.

Use `expo-secure-store` or `react-native-keychain` for tokens — never `AsyncStorage`.

Validate all deep link parameters.
