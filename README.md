# tsconfig-earlycross

This is a set of TSConfig configuration preset files for a TypeScript project, intended for use within EarlyCross.

## Install

```
npm i -D tsconfig-earlycross
```

## Configuration

Examples of `tsconfig.json`:

### Browser Module

```jsonc
{
  "extends": "tsconfig-earlycross/tsconfig",
  "include": ["src/**/*"],
  "compilerOptions": {
    "declaration": true,
    "lib": ["ESNext", "DOM"],
    "module": "ESNext"
    ...
  }
}
```

### Browser Executable

```jsonc
{
  "extends": "tsconfig-earlycross/tsconfig",
  "include": ["src/**/*"],
  "compilerOptions": {
    "removeComments": true,
    "lib": ["ESNext", "DOM"],
    "module": "ESNext"
    ...
  }
}
```

### Node Module

```jsonc
{
  "extends": "tsconfig-earlycross/tsconfig",
  "include": ["src/**/*"],
  "compilerOptions": {
    "declaration": true,
    "lib": ["ESNext"],
    "module": "CommonJS"
    ...
  }
}
```

### Node Executable

```jsonc
{
  "extends": "tsconfig-earlycross/tsconfig",
  "include": ["src/**/*"],
  "compilerOptions": {
    "removeComments": true,
    "lib": ["ESNext"],
    "module": "CommonJS"
    ...
  }
}
```
