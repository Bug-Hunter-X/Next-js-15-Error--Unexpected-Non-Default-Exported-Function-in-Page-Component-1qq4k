# Next.js 15 Unexpected Non-Default Exported Function Error

This repository demonstrates a subtle bug in Next.js 15 where the presence of a non-default exported function within a page component, even if unused, can lead to unexpected errors.  This issue is particularly relevant when migrating or upgrading from older Next.js versions.

## Steps to Reproduce

1. Clone this repository.
2. Install dependencies using `npm install`.
3. Run the development server using `npm run dev`.
4. Navigate to `/about`.

You will observe an error in your browser's console, highlighting the issue. The error is not related to the function's execution but rather its mere existence as a non-default export.

## Solution

The solution is simple: remove the function or refactor the file so that the function is a default export or not exported at all. The `aboutSolution.js` file provides a working example.