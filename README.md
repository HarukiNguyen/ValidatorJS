# ValidatorJS

## ⚠️ This project is under development

## Installation

With npm.

```bash
npm i @harukinguyen/validatorjs
```

With yarn.

```yarn
yarn add @harukinguyen/validatorjs
```

With pnpm

```pnpm
pnpm install @harukinguyen/validatorjs
```

## Usage

### HTML

First, you will need to setup your form controls in your HTML.

Currently, the library provides these HTML attributes to mark the input for what to validate.

- `validate-required`: input need to be fill.
- `s-username`: username for signup form.
- `s-password`: password for signup form.
- `email`: email.
- `confirm`: use for confirm password (need to have password input, and the password input must have `id="s-pwd"`)

⚠️ Validate logic for loging will be increase soon.

- `l-username`: username for login form.
- `l-password`: password for login form.

Example:

```HTML
<input
  type="text"
  placeholder="Enter your username..."
  validate-required
  s-username
/>
<input
  type="password"
  id="s-pwd"
  placeholder="Enter password..."
  validate-required
  s-password
/>
<input
  type="password"
  placeholder="Enter your password again..."
  validate-required
  confirm
/>
```

### Javascript

Just call the function with the list of elements, it will return an array with 2 elements.

The fist element is a boolean that say if these elements are valid or not.

The second element is an array of objects, each object contain information about the validation of the input.

Example:

```javscript
// Under testing
```

## ✅ Todo

- [ ] Add logic for handle login form.
