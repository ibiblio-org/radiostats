The frontend uses [Vite](https://vite.dev/) with React. Tests run under [Vitest](https://vitest.dev/).

## Available Scripts

### `npm start`

Runs the app in development mode. Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

### `npm test`

Runs the test suite once and exits. Uses Vitest with jsdom.

### `npm run build`

Builds the app for production to the `dist/` folder.

### `npm run preview`

Serves the production build locally for inspection.

## Notes

- JSX is used in `.js` files (CRA convention). `vite.config.js` configures esbuild to handle this.
- Tests use `vi.mock()` / `vi.clearAllMocks()` (Vitest's equivalent of Jest's `jest.mock()`).
- Runtime environment variables are injected via `public/env-config.js` at container startup, not at build time.
