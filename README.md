# Path Resolver Challenge

This project is a small JavaScript exercise focused on resolving file paths correctly.

## Problem

You are given a function named `getAbsolutePath(filePath)` in `pathResolver.js`.

The task is to make this function return the absolute path for the given file or folder path.

Example:

- Input: `src/file.txt`
- Output: `/absolute/path/to/project/src/file.txt`

The solution must work with Node.js path resolution rules and should behave correctly for relative paths.

## Files in this project

- `pathResolver.js` — contains the function to implement.
- `index.js` — a sample runner that calls the function using `src/file.txt`.
- `src/file.txt` — a sample file used for testing.
- `upload_project.js` — a helper script that packages the project into a zip and uploads it to the platform.

## What the code does

`index.js` calls:

```js
const path_to_file = path.resolve("src", "file.txt");
console.log(getAbsolutePath(path_to_file));
```

This means the program expects `getAbsolutePath()` to convert a path into a full absolute file path.

## Expected behavior

When you run:

```bash
node index.js
```

it should print the absolute path to `src/file.txt` in the current workspace.

## Notes

- The provided code is intentionally minimal.
- The core challenge is to correctly use Node.js path resolution.
- Do not change the pre-written code unless the task specifically requires it.

## Submission helper

`upload_project.js` is only for submitting the project as a zip archive. It is not part of the actual path-solving logic.

If you are working locally, you can test the challenge by running the app with Node.js and checking the output path.
