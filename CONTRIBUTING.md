# Contributing to Booild Engine

## Status

The engine source is being extracted from the Booild platform. Until the
extraction gate is green:

- **Issues and design discussions are welcome.**
- **Do not open large code PRs**; they cannot be merged until the package
  boundaries and CI are in place.
- Documentation and example contributions are welcome once the docs skeleton is
  published.

## License and sign-off

This project is licensed under the **Apache License 2.0**. By contributing, you
agree that your contribution is licensed under the same terms.

All commits must be signed off under the Developer Certificate of Origin (DCO):

```bash
git commit -s -m "feat(engine): ..."
```

The sign-off certifies that you have the right to submit the contribution under
the project licence. A CLA is not required.

## Workflow

1. Open an issue describing the change.
2. Wait for the maintainers to confirm the package boundary and approach.
3. Fork, create a branch, and add tests.
4. Run the relevant checks (published in `README.md` once the code lands).
5. Open a PR with a clear description, linked issue and test evidence.

## Code of conduct

By participating, you agree to follow [`CODE_OF_CONDUCT.md`](./CODE_OF_CONDUCT.md).

## Security

Do not report security issues in public. See [`SECURITY.md`](./SECURITY.md).
