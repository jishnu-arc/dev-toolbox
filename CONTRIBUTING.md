# Contributing

Thanks for helping improve Developer Toolbox.

## Ground rules

- Keep it dependency-free and build-free. Plain HTML, CSS and JavaScript only.
- Nothing may be sent to a server. All tools run locally.
- Keep it accessible: labels on inputs, visible focus, and keyboard support.
- Keep the code readable. Small functions and clear names.

## Adding a tool

1. Add a `<section class="tool" id="your-tool">` block in `index.html`.
2. Add `["your-tool", "Display name"]` to the `tools` array in the script.
3. Write the logic as small functions near the other tools.
4. Test in light mode, dark mode, and a narrow mobile window.
5. Add the tool to the table in `README.md`.

## Pull requests

1. Fork the repo and create a branch: `git checkout -b feature/jwt-decoder`
2. Make your change and describe it clearly in the pull request.
3. Include a screenshot for any visual change.

## Reporting bugs

Open an issue with your browser, the steps to reproduce, and the expected result.
