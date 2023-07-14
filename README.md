# ReactConfluence

ReactConfluence is a lightweight React package that allows you to seamlessly embed Confluence documentation pages into your React applications. With ReactConfluence, you can easily integrate Confluence content into your React components, providing a seamless user experience for accessing and navigating your documentation.

## Features

- Embed Confluence documentation pages into your React applications
- Customize the appearance and styling of the embedded content
- Support for dynamic rendering of Confluence pages based on user interactions

## Installation

You can install ReactConfluence using npm or Yarn. Run the following command in your project directory:

```shell
npm install react-confluence
```

or

```shell
yarn add react-confluence
```

## Usage

To use ReactConfluence, follow these simple steps:

1. Import the necessary components from the `react-confluence` package:

```javascript
import { ConfluencePage } from "react-confluence";
```

2. Use the `ConfluencePage` component in your React component, providing the required props:

```jsx
<ConfluencePage pageUrl="<confluence_page_url>" apiKey="<confluence_api_key>" />
```

Replace `<confluence_page_url>` with the URL of the Confluence page you want to embed, and `<confluence_api_key>` with your Confluence API key.

3. Customize the appearance and behavior of the embedded content by passing additional props to the `ConfluencePage` component. For example:

```jsx
<ConfluencePage
  pageUrl="<confluence_page_url>"
  apiKey="<confluence_api_key>"
  width="100%"
  height="500px"
  showControls={false}
  theme="dark"
/>
```

4. Enjoy the seamless integration of Confluence documentation pages within your React application!

## Props

The `ConfluencePage` component accepts the following props:

- `pageUrl` (required): The URL of the Confluence page you want to embed.
- `apiKey` (required): Your Confluence API key for authentication.
- `width` (optional): The width of the embedded content. Default is `'100%'`.
- `height` (optional): The height of the embedded content. Default is `'100%'`.
- `showControls` (optional): Whether to show navigation controls for the embedded content. Default is `true`.
- `theme` (optional): The color theme of the embedded content. Supported values are `'light'` and `'dark'`. Default is `'light'`.

## Examples

Here's an example of embedding a Confluence page into a React component:

```jsx
import React from "react";
import { ConfluencePage } from "react-confluence";

const MyDocumentationComponent = () => {
  const pageUrl = "<confluence_page_url>";
  const apiKey = "<confluence_api_key>";

  return (
    <div>
      <h1>My Documentation</h1>
      <ConfluencePage pageUrl={pageUrl} apiKey={apiKey} />
    </div>
  );
};

export default MyDocumentationComponent;
```

## Contributions

Contributions to ReactConfluence are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the [GitHub repository](https://github.com/yourusername/ReactConfluence).

## License

This project is licensed under the [MIT License](LICENSE).
