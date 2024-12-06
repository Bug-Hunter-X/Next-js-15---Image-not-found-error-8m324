# Next.js 15 - Image not found error

This repository demonstrates a common error in Next.js 15 applications where an image is not found in the /public directory.  The error message is not very helpful, and this example shows how to reproduce and fix the issue.

## Bug
The `pages/about.js` component attempts to render an image using the `img` tag.  However, the image file does not exist in the /public directory, leading to an error.

## Solution
The solution involves either creating the image file in the /public directory or removing the problematic `img` tag from `pages/about.js`. Alternatively, error handling could be introduced to gracefully handle the missing image.

## Reproduction
1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Navigate to `/about`.
5. Observe the error in the browser console.
