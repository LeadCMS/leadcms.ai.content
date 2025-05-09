# Copilot Instructions for Creating New Pages and Posts

## Overview
This document provides guidelines for creating new pages and posts in the LeadCMS content repository. The content is organized into folders under the `content` directory, with each folder representing a specific type of content (e.g., `home`, `post`, `legal`, `contact`). Each page or post typically consists of an `index.mdx` file and a mandatory `index.json` file for metadata.

---

## General Structure
1. **Folder Naming**: Each new page or post should have its own folder under the appropriate category (e.g., `content/post/new-post/`).
2. **Files**:
   - `index.mdx`: The main content file written in MDX format.
   - `index.json`: Mandatory metadata file for additional configuration or SEO.
3. **Assets**: Any images or media files should be placed in the same folder as the `index.mdx` file.

---

## Creating a New Page
1. **Choose the Category**: Determine the appropriate category for the new page (e.g., `home`, `legal`, `contact`).
2. **Create a Folder**: Add a new folder under the chosen category with a descriptive name (e.g., `content/contact/support/`).
3. **Add `index.mdx`**:
   - Start with a frontmatter block for SEO metadata (e.g., `SeoKeywords`, `SeoTitle`, `SeoDescription`).
   - Use consistent MDX components (e.g., `section`, `Card`, `Badge`).
   - Follow the design patterns used in existing pages.
4. **Add `index.json`**:
   - Include metadata such as `title`, `description`, `author`, `language`, `category`, `tags`, and `publishedAt`.
   - Ensure all required fields are filled out.

---

## Creating a New Post
1. **Navigate to `content/post/`**: All posts are stored in the `post` folder.
2. **Create a Folder**: Add a new folder with a descriptive name (e.g., `content/post/new-feature/`).
3. **Add `index.mdx`**:
   - Include a frontmatter block with `SeoTitle` and `SeoDescription`.
   - Use a consistent structure with headings, paragraphs, and components like `Badge` and `Card`.
   - Add a summary section at the beginning.
4. **Add `index.json`**:
   - Use this file for metadata such as `title`, `description`, `author`, `language`, `category`, `tags`, and `publishedAt`.
   - Ensure all required fields are filled out.
5. **Add Media Files**:
   - Place any images or media files in the same folder.
   - Use descriptive filenames (e.g., `new-feature.png`).

---

## Key Libraries and Technologies
1. **CSS Framework**:
   - The project uses TailwindCSS for styling. Use utility classes like `bg-primary`, `text-muted-foreground`, `rounded-xl`, etc., to maintain consistency.

2. **Reusable Components**:
   - Leverage existing components such as `Card`, `Badge`, `Button`, and icons like `CheckCircle`, `Users`, `Shield`, etc., for a consistent design.

3. **Frontend Framework**:
   - React is the primary framework for building UI components. Ensure all new components follow React's best practices.

4. **Markdown with JSX (MDX)**:
   - Write content in MDX format to combine Markdown with React components. This allows for dynamic and interactive content.

5. **SEO Metadata**:
   - Include `SeoTitle`, `SeoDescription`, and `SeoKeywords` in the frontmatter of MDX files for SEO optimization.

6. **Localization**:
   - Ensure all content is written in Russian and uses consistent terminology to align with the project's localization strategy.

7. **Git-based CMS**:
   - Follow the Git-based approach for content management. All changes should be version-controlled, and content should be structured for easy collaboration and rollback.

---

## Best Practices
1. **SEO Optimization**:
   - Use meaningful `SeoTitle` and `SeoDescription` in the frontmatter.
   - Include relevant `SeoKeywords`.
2. **Consistent Design**:
   - Follow the design patterns and components used in existing files.
   - Use reusable components like `Card`, `Badge`, and `Button`.
3. **Localization**:
   - Ensure content is written in the appropriate language.
   - Use consistent terminology.
4. **Testing**:
   - Preview the page or post locally to ensure proper rendering.
   - Check for broken links and missing assets.

---

## Example Frontmatter for `index.mdx`
```mdx
---
SeoTitle: "Title of the Page or Post"
SeoDescription: "Brief description for SEO purposes."
SeoKeywords: "keyword1, keyword2, keyword3"
---
```

Please never add comments like {/* comments */} and empty lines in the mdx files.

---

## Example Folder Structure for a Post
```
content/post/example-post/
├── index.mdx
├── index.json
└── example-post.png (optional)
```