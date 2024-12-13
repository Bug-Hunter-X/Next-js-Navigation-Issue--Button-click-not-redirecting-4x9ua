# Next.js Navigation Bug

This repository demonstrates a common navigation issue in Next.js applications where a navigation action (in this case, a button click) fails to trigger the expected page transition.  The issue is that there is no error shown in the console which makes it hard to track down.

## The Bug

The application consists of two pages: `index.js` (home page) and `about.js` (about page).  A link on the home page navigates to the about page. On the about page, a button should navigate back to the home page.  However, the button click does not redirect the user, despite seemingly correct usage of `useRouter.push()`.

## Reproduction Steps

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Navigate to the `/about` page using the link on the home page.
5. Click the 'Go back to Home' button; you will notice that it does not redirect to the home page.

## Solution

The solution is available in the `solution` branch.