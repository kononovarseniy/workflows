# Reusable GitHub Workflows

Repository containing reusable GitHub workflows.

Use semantic version tags (e.g., `@v1.0.0`) when referencing workflows.

## Available Workflows

### [`conan-multi-platform.yml`](.github/workflows/conan-multi-platform.yml)
Builds Conan 2 package across multiple platforms with caching support. Builds on:
- Ubuntu (Clang 18, GCC 14)
- macOS (Apple Clang 16)
- Windows (MSVC 2022)

### Usage
```yml
name: 🔨 Build

on:
  workflow_dispatch:

jobs:
  build:
    uses: kononovarseniy/workflows/.github/workflows/conan-multi-platform.yml@v1.0.0
```

## License
MIT License. See [LICENSE](LICENSE) file for details.
