# React Router Dom Unexpected Behavior with Anchor Tags

This repository demonstrates an unexpected behavior in React Router Dom when using anchor tags (<a>) instead of the provided Link component for navigation within the application.  While both seem to perform the same initial navigation, the use of the anchor tag triggers an unnecessary full page reload, which can negatively impact the user experience and SEO. This example highlights the importance of consistently using the Link component for internal navigation in React Router applications.

## Problem

When using the standard HTML anchor tag (<a>) with a relative path (e.g., `/about`), the browser performs a full page reload, rather than updating only the content within the router's context.

## Solution

To avoid this behavior, ensure you always use the `Link` component provided by `react-router-dom` for internal navigation within your application. The Link component is specifically designed to work with React Router, providing seamless updates to the application's state without full-page reloads.