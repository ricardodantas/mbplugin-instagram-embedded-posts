# Instagram Embed Plugin for Micro.blog

This is a Micro.blog plugin that allows you to easily embed Instagram posts and reels in your Micro.blog posts using Instagram URLs.

## Usage

### Basic Usage

To embed an Instagram post, use the shortcode with the Instagram URL:

```
{{< instagram "https://www.instagram.com/p/POST_ID/" >}}
```

### With Custom Caption

You can add a custom caption that will appear below the embedded post:

```
{{< instagram "https://www.instagram.com/p/POST_ID/" caption="Check out this amazing post!" >}}
```

### Hide Instagram Caption

To hide the original Instagram caption, use the `hidecaption` parameter:

```
{{< instagram "https://www.instagram.com/p/POST_ID/" hidecaption="true" >}}
```

### Supported URL Formats

The plugin supports both Instagram posts and reels:

- Posts: `https://www.instagram.com/p/POST_ID/`
- Reels: `https://www.instagram.com/reel/REEL_ID/`

## Features

- **Automatic URL parsing**: Extracts the post ID from various Instagram URL formats
- **Responsive design**: Embeds are mobile-friendly and responsive
- **Custom captions**: Add your own captions to provide context
- **Caption control**: Option to hide original Instagram captions
- **Fallback display**: Shows a styled placeholder that looks like an Instagram post even before the JavaScript loads
- **Error handling**: Provides clear error messages for invalid URLs

## Technical Details

The plugin uses Instagram's official embed API and includes:

- Instagram's embed JavaScript for dynamic loading
- Fallback styling that matches Instagram's design
- Proper error handling for invalid URLs
- Support for both posts and reels

## Examples

### Simple embed

```
{{< instagram "https://www.instagram.com/p/ABC123/" >}}
```

### With custom caption

```
{{< instagram "https://www.instagram.com/p/ABC123/" caption="Great inspiration for today!" >}}
```

### Reel with hidden caption

```
{{< instagram "https://www.instagram.com/reel/XYZ789/" hidecaption="true" >}}
```

## Troubleshooting

- **Invalid URL error**: Make sure you're using a valid Instagram post or reel URL
- **Post not loading**: Ensure the Instagram post is public and not deleted
- **Styling issues**: The embedded post inherits your site's styling; you may need to adjust CSS for optimal display

## License

This project is licensed under the [Apache License 2.0](LICENSE).
