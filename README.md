# Instagram Embed Plugin for Micro.blog

This is a Micro.blog plugin that allows you to easily embed Instagram posts and reels in your Micro.blog posts using Instagram URLs.

## Usage

### Basic Usage

To embed an Instagram post, use the shortcode with the Instagram URL:

```
{{< instagram "ABC123def456" >}}
```

### With Custom Caption

You can add a custom caption that will appear below the embedded post:

```
{{< instagram "ABC123def456" caption="Check out this amazing post!" >}}
```

### Hide Instagram Caption

To hide the original Instagram caption, use the `hidecaption` parameter:

```
{{< instagram "ABC123def456" hidecaption="true" >}}
```

## Troubleshooting

- **Post not loading**: Ensure the Instagram post is public and not deleted
- **Styling issues**: The embedded post inherits your site's styling; you may need to adjust CSS for optimal display

## License

This project is licensed under the [Apache License 2.0](LICENSE).
