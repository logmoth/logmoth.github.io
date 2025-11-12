# Adding Images to Blog Posts

## Where to Store Images

Store your images in the `assets/images/` directory. This directory has been created for you.

## How to Add Images in Markdown

### Basic Syntax

```markdown
![Alt text describing the image](/assets/images/your-image.jpg)
```

### With Title (Optional)

```markdown
![Alt text](/assets/images/your-image.jpg "Image title")
```

### With Link (Clickable Image)

```markdown
[![Alt text](/assets/images/your-image.jpg)](https://example.com)
```

### Using Relative Paths

If your image is in the same directory as your post, you can use:

```markdown
![Alt text](./image.jpg)
```

However, it's recommended to use the `/assets/images/` path for consistency.

## Example

Here's an example from a blog post:

```markdown
## My Project

Here's a screenshot of my project:

![Project Screenshot](/assets/images/project-screenshot.png)

As you can see, it's amazing!
```

## Supported Image Formats

Jekyll supports all common image formats:
- `.jpg` / `.jpeg`
- `.png`
- `.gif`
- `.svg`
- `.webp`

## Tips

1. **Optimize your images** - Large images can slow down your site. Use tools like TinyPNG or ImageOptim to compress images before uploading.

2. **Use descriptive alt text** - This helps with accessibility and SEO.

3. **Organize your images** - You can create subdirectories in `assets/images/` to organize images by post or date, e.g.:
   - `assets/images/2025/11/my-image.jpg`
   - `assets/images/projects/project1.png`

4. **Referencing from posts** - Since your posts are in `_posts/`, you can reference images using:
   - Absolute path: `/assets/images/image.jpg` (recommended)
   - Jekyll's `relative_url` filter: `{{ "/assets/images/image.jpg" | relative_url }}` (for more complex cases)

