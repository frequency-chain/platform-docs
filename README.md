# Platform Documentation

This repository contains our documentation, which is automatically synced to [GitBook.com](https://gitbook.com). The documentation is written in Markdown and follows a specific structure to work with GitBook's GitHub integration.

## Important Note

**Any changes pushed to the `main` branch will automatically sync to GitBook.com.** This means:

- All documentation changes should be made through pull requests
- Changes are only published when merged to `main`
- The `main` branch is the source of truth for the live documentation

## Repository Structure (current needs to be change, this was my sample)

- `docs/` - Contains all documentation files
  - `getting-started/` - Getting started guides
  - `guides/` - Detailed guides and tutorials
  - `api/` - API documentation
  - `contributing/` - Contributing guidelines
- `SUMMARY.md` - Defines the documentation structure and navigation
- `README.md` - This file (appears as the introduction in GitBook)

## How It Works

1. **Documentation Structure**

   - The `SUMMARY.md` file defines the table of contents and navigation structure
   - Each entry in `SUMMARY.md` links to a Markdown file in the `docs/` directory
   - The structure in `SUMMARY.md` determines the order and hierarchy in GitBook

2. **GitBook Integration**

   - This repository is connected to GitBook.com via GitHub integration
   - Changes pushed to this repository are automatically synced to GitBook
   - The documentation is published and hosted on GitBook.com

3. **Writing Documentation**
   - All documentation is written in Markdown (`.md` files)
   - Files should be placed in the appropriate directory under `docs/`
   - Add new pages to `SUMMARY.md` to include them in the navigation
   - Use relative links between documentation files

## Contributing

We welcome contributions to our documentation! Please feel free to submit pull requests or open issues for any improvements or corrections.

1. Fork the repository
2. Create a new branch for your changes
3. Make your changes
4. Submit a pull request
5. Once approved and merged to `main`, changes will automatically sync to GitBook

## License

This documentation is open source and available under the same license as our main project.
