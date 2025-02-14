# Changelog

## v2.0.2 - 2022-04-14

### Changed

- Updated [react-document-portal](https://www.npmjs.com/package/react-document-portal) dependency to v1.2.1.
- Updated [react-use-keypress](https://www.npmjs.com/package/react-document-portal) dependency to v1.3.1.
- Updated [react](https://www.npmjs.com/package/react) and [react-dom](https://www.npmjs.com/package/react-dom) peer-dependencies to support v18.

## v2.0.1 - 2021-12-15

### Added

- Added [react-dom](https://www.npmjs.com/package/react-dom) peer-dependency.

### Changed

- Updated [react-document-portal](https://www.npmjs.com/package/react-document-portal) dependency to v1.2.0.

## v2.0.0 - 2021-12-14

### Changed

- **BREAKING** Changed JSX transform to use new React JSX runtime.

### Removed

- Removed `propTypes` property from components.

## v1.6.0 - 2020-09-25

### Changed

- Updated `propTypes` to only be defined in non-production environments.
- Updated React import to avoid using default import.
- Updated styles to use numbers (instead of strings) where possible.

## v1.5.0 - 2020-09-05

### Added

- Added background to loading state that matches iframe contents.

### Changed

- Improved labels for screen readers and other assistive technologies.
- Replaced styles from injected CSS to inline styles for better SSR support.
- Replaced CSS animation of spinner with SVG animation inside [spinner.svg](./src/spinner.svg).
- Updated [close.svg](./src/close.svg) to no longer have textured background.

### Removed

- Removed [@babel/runtime](https://www.npmjs.com/package/@babel/runtime) dependency for Babel helpers.
- Removed error handler for iframe and always display iframe and close button.
- Removed explicit [react-dom](https://www.npmjs.com/package/react-dom) peer-dependency.

## v1.4.1 - 2020-09-04

### Fixed

- Added checks to ensure nodes exist before calling DOM methods.
- Fixed a bug where the shielded button would try gain focus on mount.

## v1.4.0 - 2020-09-02

### Changed

- Changed how `overflow` style on `<body>` element is reverted to prevent taking higher specificity over app styles.
- Replaced internal `Portal` component with [react-document-portal](https://www.npmjs.com/package/react-document-portal).
- Replaced all uses of `useLayoutEffect` hook with `useEffect` hook.

## v1.3.0 - 2020-07-10

### Added

- Added [@babel/runtime](https://www.npmjs.com/package/@babel/runtime) for Babel helpers.

### Changed

- Bumped up version of [react-use-keypress](https://www.npmjs.com/package/react-use-keypress) to v1.0.1.
- Reduced build output of SVG components.

## v1.2.0 - 2020-05-19

### Added

- Added ES Module build.

### Changed

- Enabled loose mode on '@babel/preset-env' to reduce build output.
- Replaced internal `useEscapeKey` hook with [react-use-keypress](https://www.npmjs.com/package/react-use-keypress).

### Removed

- Removed [prop-types](https://www.npmjs.com/package/prop-types), as `Shielded` component doesn't have props.

## v1.1.0 - 2020-04-27

### Changed

- Update URLs to new staticcdn.co.nz domain.

### Fixed

- Fixed a bug in internal `useEscapeKey` hook.

## v1.0.0 - 2019-10-26

Initial public version! :tada:
