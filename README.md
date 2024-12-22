# Tailwind CSS Styles Not Applying in Next.js/Nuxt.js Components

This repository demonstrates a common issue where Tailwind CSS styles fail to apply to components in Next.js or Nuxt.js projects, even when the configuration appears correct. The problem lies in how Tailwind processes the CSS at build time and the order of operations within the framework.

## Reproducing the Bug

1. Clone this repository.
2. Install dependencies: `npm install`
3. Run the development server.  Observe that the component in `bug.jsx` lacks the expected Tailwind styles.

## Solution

The `bugSolution.jsx` file demonstrates the fix by ensuring that Tailwind's purge process includes the necessary components.  Specific solutions will depend on your framework but usually involve making sure your Tailwind configuration correctly identifies the files containing the classes you are using.