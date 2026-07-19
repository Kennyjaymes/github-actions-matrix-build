# Matrix Build Demo

This is a simple demonstration project for testing GitHub Actions matrix builds.

## Overview

The project consists of a simple Node.js script exporting an `add` function, and it uses `jest` to run unit tests.

The main purpose of this repository is to demonstrate how to configure and run a GitHub Actions workflow using a build matrix.

## GitHub Actions Matrix Build

The included workflow (`.github/workflows/matrix-build.yml`) runs tests automatically on pushes and pull requests to the `main` branch. 

It is configured to run across a matrix of multiple Operating Systems and Node.js versions:

**Operating Systems:**
- `ubuntu-latest`
- `windows-latest`
- `macos-latest`

**Node.js Versions:**
- `18`
- `20`
- `22`

This ensures that the code functions correctly across 9 different environment combinations.

## Running Tests Locally

To run the tests locally, make sure you have Node.js installed.

1. Install dependencies:
   ```bash
   npm install
   ```

2. Run the tests:
   ```bash
   npm test
   ```
