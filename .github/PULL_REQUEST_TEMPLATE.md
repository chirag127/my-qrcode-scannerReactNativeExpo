# Pull Request Template

## Description

Provide a concise summary of the changes introduced in this pull request.

## Type of Change

- [ ] Bug fix (non-breaking change which fixes an issue)
- [ ] New feature (non-breaking change which adds functionality)
- [ ] Breaking change (fix or feature that would cause existing functionality to not work as expected)
- [ ] Documentation update
- [ ] Refactor
- [ ] Performance Improvement

## Checklist

- [ ] I have read and understood the **CONTRIBUTING.md** guidelines.
- [ ] My code adheres to the **Apex Technical Authority** standards and architectural principles.
- [ ] I have performed a self-review of my own code.
- [ ] I have commented my code, particularly in hard-to-understand areas.
- [ ] I have made corresponding changes to the documentation (if applicable).
- [ ] My changes generate no new warnings or errors.
- [ ] I have added tests that prove my fix is effective or that my feature works.
- [ ] New and existing unit tests pass locally with my changes.
- [ ] Any dependent components have been updated or released.
- [ ] I have updated the **AGENTS.md** documentation if my changes impact AI agent directives or tooling.

## Related Issues

Closes #

## Technical Notes & Architectural Alignment

*   **Architecture:** Changes align with the established **Feature-Sliced Design (FSD)** principles for React Native projects. (See AGENTS.md for details).
*   **Tooling:** All development and testing adhere to the **Apex Toolchain**: TypeScript, Vite, TailwindCSS v4, Tauri v2, Biome, Vitest, Playwright.
*   **Performance:** Focus on maintaining or improving the high-performance characteristics of the `ScanFlow-HighPerformance-QRBarcode-MobileScanner-App`.
*   **Data Integrity:** Ensure all data capture and processing are accurate and resilient.
*   **Security:** Follows the guidelines outlined in **SECURITY.md**.

## Additional Context

Add any other context about the problem that you want to provide.

--- 

**IMPORTANT:** Ensure all changes are validated against the **Apex Technical Authority** standards and the project's core directives as detailed in **AGENTS.md**. Verify all dynamic links and badges reflect the correct repository name: `https://github.com/chirag127/ScanFlow-HighPerformance-QRBarcode-MobileScanner-App`.