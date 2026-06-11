# @hakatashi/oxlint-config

Koki Takahashi's shared [oxlint](https://oxc.rs/docs/guide/usage/linter.html) configuration.

Ports the rule philosophy from [@hakatashi/eslint-config](https://github.com/hakatashi/eslint-config) to oxlint's config format.

## Installation

```sh
npm install --save-dev @hakatashi/oxlint-config oxlint
```

## Usage

### `oxlint.config.ts` (recommended)

Requires Node.js v22.18+ or v24+.

```typescript
import config from '@hakatashi/oxlint-config';
import {defineConfig} from 'oxlint';

export default defineConfig({
	extends: [config],
});
```

### `.oxlintrc.json`

```json
{
	"extends": ["./node_modules/@hakatashi/oxlint-config/index.json"]
}
```

## Included plugins

- **eslint** (default) — JavaScript built-in rules
- **react** — React/JSX rules
- **import** — ES module import rules
- **node** — Node.js-specific rules

## License

MIT
