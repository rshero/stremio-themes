# Stremio Themes

Custom CSS themes for [Stremio Web](https://web.stremio.com).

## Usage

1. Open Stremio Web (or Stremio Desktop with web UI)
2. Go to **Settings** > **Appearance**
3. Enter a theme URL from the table below
4. Click **Apply Theme**

## Available Themes

| Theme | Description | URL |
|-------|-------------|-----|
| [Catppuccin Mocha](themes/catppuccin-mocha.css) | Warm, cozy dark theme with pastel colors | `https://raw.githubusercontent.com/USER/stremio-themes/main/themes/catppuccin-mocha.css` |

> Replace `USER` with your GitHub username in the URLs above.

## Creating Your Own Theme

Themes work by overriding CSS custom properties and adding style overrides.

### Basic Structure

```css
:root {
    /* Backgrounds */
    --primary-background-color: #1e1e2e;
    --secondary-background-color: #181825;
    
    /* Text colors */
    --primary-foreground-color: #cdd6f4;
    --secondary-foreground-color: #1e1e2e;
    
    /* Accent colors */
    --primary-accent-color: #cba6f7;
    --secondary-accent-color: #a6e3a1;
    --tertiary-accent-color: #f9e2af;
    --quaternary-accent-color: #89b4fa;
    
    /* UI elements */
    --modal-background-color: #313244;
    --overlay-color: rgba(69, 71, 90, 0.6);
    
    /* Status colors */
    --warning-accent-color: #fab387;
    --danger-accent-color: #f38ba8;
    
    /* Effects */
    --outer-glow: 0px 0px 15px rgba(203, 166, 247, 0.3);
    --border-radius: 0.75rem;
}

/* Additional overrides as needed */
```

### Tips

- Use `!important` for overrides that need to take precedence
- Test your theme across different pages (library, discover, player, settings)
- Check both light and dark system themes if applicable

## Contributing

1. Fork this repository
2. Create your theme in the `themes/` directory
3. Add a preview screenshot to `previews/` (optional)
4. Update the README with your theme
5. Submit a pull request

## License

MIT
