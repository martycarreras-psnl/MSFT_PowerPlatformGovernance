# Contributing

This project welcomes contributions and suggestions. Most contributions require you to
agree to a Contributor License Agreement (CLA) declaring that you have the right to,
and actually do, grant us the rights to use your contribution. For details, visit
https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need
to provide a CLA and decorate the PR appropriately (e.g., status check, comment). Simply
follow the instructions provided by the bot. You will only need to do this once across
all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/)
or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Getting Started

This repository is a set of static HTML reference pages — no build step, no dependencies.

1. **Fork the repository** and clone your fork locally.
2. **Open `index.html` or `first-90-days.html`** directly in a browser to preview changes.
3. **Make your changes** on a feature branch.
4. **Open a pull request** against `main`.

## What We're Looking For

- Factual corrections to Power Platform governance guidance (license SKUs, connector names, PPAC paths, throttle limits, API versions)
- New or improved decision lenses, stage actions, or admin-agent pro tips
- Accessibility improvements (semantic HTML, ARIA, color contrast)
- Print-stylesheet and dark-theme polish
- Documentation clarity and typo fixes
- Cross-browser compatibility fixes

## Guidelines

### Content Style

- Cite Microsoft Learn or official PPAC docs for any prescriptive claim (license SKUs, connector action names, API versions).
- Do **not** reference the deprecated CoE Toolkit; this guide is built on tenant-native primitives (PPAC, Managed Environments, Environment Groups, Recommendations) and Power Platform admin connectors.
- Match the existing voice — direct, prescriptive, no marketing fluff.
- Preserve the Clawpilot theme variables (`--cp-*`, `--zone1/2/3`) — do not introduce hardcoded colors.

### Commits

- Use conventional commit messages: `fix:`, `feat:`, `chore:`, `docs:`.
- One logical change per commit. Squash fixup commits before merging.

### Validation

- Open the page in both light and dark themes (`?clawpilotTheme=light` / `?clawpilotTheme=dark`) and verify no contrast regressions.
- Test the print stylesheet (`Cmd/Ctrl+P` → preview).
- Confirm interactive elements (self-assessment, action checkboxes, Export Summary modal) still work after JS changes.

## Pull Request Checklist

- [ ] Changes render cleanly in both light and dark themes
- [ ] Any new prescriptive claim cites a Microsoft Learn / PPAC source in the PR description
- [ ] No hardcoded colors — uses existing CSS variables
- [ ] No references to deprecated CoE Toolkit
- [ ] No secrets or credentials in the diff
- [ ] Commit messages follow conventional format
- [ ] PR description explains the why, not just the what

## Reporting Issues

Open a GitHub issue with:
- What you expected to see
- What actually appeared
- Steps to reproduce (browser, theme, page)

For security vulnerabilities, see [SECURITY.md](SECURITY.md).
