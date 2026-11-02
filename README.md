# prettier

The code style of AYÇİÇEK Labs. Every file Prettier can format follows it.

| File              | Purpose                                                                       |
| ----------------- | ----------------------------------------------------------------------------- |
| `.prettierrc`     | 100-column lines, single quotes, trailing commas everywhere, LF line endings. |
| `.prettierignore` | Committed files written by tools: lock files, `CHANGELOG.md`, minified files. |

Everything else uses Prettier's defaults. Prettier also skips every path in `.gitignore`.

## Use it in a project

```sh
base=https://raw.githubusercontent.com/AYCICEK-Labs/prettier/main
curl -fsSL "$base/.prettierrc" -o .prettierrc
curl -fsSL "$base/.prettierignore" -o .prettierignore
```

Check or format every file:

```sh
npx prettier --check .
npx prettier --write .
```

## License

[MIT](LICENSE) © Yunus Emre AYÇİÇEK
