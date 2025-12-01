# CONTRIBUTING GUIDELINES

Welcome to the ScanFlow Mobile Scanner Utility! We are thrilled you're interested in contributing to this high-performance, cross-platform mobile application.

Our mission is to deliver a **zero-defect, high-velocity, future-proof** mobile data capture solution. To maintain this standard and ensure a smooth contribution process, please adhere to the following guidelines.

## 1. CODE OF CONDUCT

By participating, you are expected to uphold our **Code of Conduct**. This ensures a welcoming and respectful environment for all contributors.

## 2. DEVELOPMENT ENVIRONMENT SETUP

To contribute, you'll need to set up your local development environment. We leverage **React Native** and **Expo** for cross-platform development.

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/your-username/scanflow-mobile-scanner-utility.git
    cd scanflow-mobile-scanner-utility
    ```

2.  **Install Node.js & npm/yarn:** Ensure you have Node.js (LTS recommended) and npm or yarn installed.

3.  **Install Project Dependencies:**
    ```bash
    npm install
    # or
    yarn install
    ```

4.  **Install Expo CLI:**
    ```bash
    npm install -g expo-cli
    # or
    yarn global add expo-cli
    ```

5.  **Start the Development Server:**
    ```bash
    npx expo start
    ```

6.  **Run on Device/Simulator:** Use the Expo Go app on your physical device or an emulator/simulator to test your changes.

## 3. BRANCHING STRATEGY

We follow a simplified Gitflow-like branching strategy:

*   **`main`**: Production-ready code. **DO NOT** commit directly to `main`.
*   **`develop`**: Integration branch for new features and fixes. This is where most development happens.
*   **Feature Branches**: Create branches from `develop` for new features or bug fixes. Use descriptive names (e.g., `feature/qr-code-scanner-optimization`, `fix/barcode-decoding-accuracy`).
    ```bash
    git checkout develop
    git pull origin develop
    git checkout -b feature/your-feature-name
    ```

## 4. CONTRIBUTION WORKFLOW

1.  **Fork the Repository**: Fork the `scanflow-mobile-scanner-utility` repository to your GitHub account.
2.  **Clone Your Fork**: Clone your forked repository locally.
3.  **Create a Branch**: Create a new branch for your contribution (see Branching Strategy).
4.  **Implement Changes**: Write your code, ensuring it adheres to our coding standards.
5.  **Test Thoroughly**: Run all tests to ensure no regressions are introduced. If you're adding new functionality, write new tests.
    ```bash
    # Example test commands (adjust as per your project's test setup)
    npm test
    # or
    yarn test
    ```
6.  **Lint & Format**: Ensure your code is linted and formatted correctly.
    ```bash
    # Example lint/format commands (adjust as per your project's setup)
    npm run lint -- --fix
    npm run format -- --write
    # or
    yarn lint --fix
    yarn format --write
    ```
7.  **Commit Your Changes**: Use **Conventional Commits** for your commit messages.
    ```bash
    # Example:
    git commit -m "feat(scanner): Improve QR code decoding performance"
    git commit -m "fix(decoder): Resolve issue with EAN-13 barcode parsing"
    ```
8.  **Push to Your Fork**: Push your branch to your forked repository.
    ```bash
    git push origin feature/your-feature-name
    ```
9.  **Create a Pull Request (PR)**: Open a Pull Request from your feature branch to the `develop` branch of the **original** `scanflow-mobile-scanner-utility` repository.
    *   **Title**: Follow the Conventional Commits format.
    *   **Description**: Clearly explain the changes, the problem solved, and how to test them. Reference any related issues.

## 5. CODING STANDARDS

We adhere to strict coding standards to maintain code quality and consistency:

*   **Language**: JavaScript (ESNext), with React Native conventions.
*   **Style**: Follow standard React Native and Expo best practices.
*   **Linting**: `Biome` will be used for linting and formatting. Ensure your code passes `biome check --apply` before committing.
*   **Testing**: `Vitest` and `Playwright` will be used for unit and E2E testing, respectively. Aim for high test coverage.
*   **SOLID Principles**: Strive to apply SOLID principles where applicable.
*   **DRY (Don't Repeat Yourself)**: Avoid code duplication.
*   **KISS (Keep It Simple, Stupid)**: Prefer straightforward solutions.
*   **Readability**: Write clear, concise, and self-documenting code. Avoid excessive comments; the code should explain itself.
*   **Error Handling**: Implement robust error handling and logging. Apps should **never crash**.

## 6. TESTING REQUIREMENTS

*   **Unit Tests**: Write unit tests for all new components, logic, and utilities using `Vitest`.
*   **Integration Tests**: For interactions between components or modules.
*   **End-to-End (E2E) Tests**: Use `Playwright` to test critical user flows on target platforms.
*   **Coverage**: Aim for a high test coverage (e.g., 90%+). Every source file should have corresponding tests.

## 7. COMMIT MESSAGE FORMAT

We use **Conventional Commits** for a structured and understandable commit history.

```
<type>[optional scope]: <description>

[optional body]

[optional footer]
```

*   **Types**: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `chore`.
*   **Scope**: The part of the codebase affected (e.g., `scanner`, `decoder`, `ui`).
*   **Description**: Concise summary of the change.
*   **Body**: More detailed explanation (optional).
*   **Footer**: For breaking changes (`BREAKING CHANGE:`) or issue references (`Closes #123`).

## 8. REPORTING BUGS

If you find a bug, please check if it has already been reported. If not, open a new **Bug Report** issue using the provided template.

## 9. REQUESTING FEATURES

To request a new feature, please open a new issue using the **Feature Request** template.

## 10. PULL REQUEST REVIEW PROCESS

*   Your PR will be reviewed by at least one maintainer.
*   Be prepared to make changes based on feedback.
*   The goal is constructive collaboration to improve the codebase.

## 11. THANK YOU!

Thank you for contributing to ScanFlow Mobile Scanner Utility! Your efforts help us build a premier mobile data capture solution.