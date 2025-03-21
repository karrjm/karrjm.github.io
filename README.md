# Website Component Guide

This guide explains how to use the simplified components in this website.

## Project Component

The Project component is a reusable element that displays a single project with an image, title, materials list, and description.

To add more projects, copy the following HTML and paste it in the `content` div in `index.html`:

```html
<article class="project-component">
  <figure class="image-container">
    <img src="YOUR_IMAGE_URL_HERE"
      alt="Descriptive alt text for accessibility" width="800"
      height="600" loading="lazy" />
  </figure>
  <h2 class="item-title">Your Project Title, Year</h2>
  <p class="item-materials">Materials list, dimensions, duration, etc.</p>
  <p class="item-description">
    Detailed description of your project. This can be multiple sentences explaining
    the concept, execution, and significance of the work.
  </p>
</article>
```

## Process Cluster Component

The Process Cluster component is a flexible element that can contain one or more images with captions, arranged in different layouts.

To add more process clusters, copy the following HTML and paste it in the `process-content` div in `index.html`:

```html
<div class="process-cluster-component">
  <!-- Main cluster container -->
  <div class="process-cluster">
    <!-- Image 1 -->
    <article class="process-item">
      <figure class="image-container">
        <img src="YOUR_IMAGE_URL_HERE" 
          alt="Descriptive alt text for accessibility"
          loading="lazy" width="800" height="600" />
      </figure>
      <p class="item-description">Optional caption for this image</p>
    </article>

    <!-- Image 2 (optional) -->
    <article class="process-item">
      <figure class="image-container">
        <img src="YOUR_IMAGE_URL_HERE" 
          alt="Descriptive alt text for accessibility"
          loading="lazy" width="800" height="600" />
      </figure>
      <p class="item-description">Optional caption for this image</p>
    </article>
  </div>
  
  <!-- Optional: Supporting text for the cluster -->
  <p class="process-text">
    Optional text describing this process stage or offering insight
  </p>
</div>
```

### Process Cluster Variations

You can customize the appearance of process-items with these CSS classes:

- `small` - 40% width, aligned left
- `medium` - 55% width, aligned right
- `large` - 70% width, centered
- `centered` - 50% width, centered

Example:
```html
<article class="process-item large">
  <!-- Image content -->
</article>
```

For the process text, you can use these variations:
- `small` - 40% width
- `large` - 75% width, larger font size

Example:
```html
<p class="process-text large">
  Important statement about your process
</p>
```
