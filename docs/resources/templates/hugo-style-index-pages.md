---
title: Creating Hugo-Style Index Pages
description: A guide for creating category index pages with automatic child page listings
sidebar_position: 5
---

# Creating Hugo-Style Index Pages

This guide explains how to create "Hugo-style" index pages in this Docusaurus site. Hugo-style index pages automatically display all child pages and subcategories in a card-based layout, making it easy for users to navigate through sections of the documentation.

## What is a Hugo-Style Index Page?

A Hugo-style index page is a category index page that automatically lists all its child pages and subcategories using a visual card layout. This pattern is common in Hugo static sites and provides an intuitive way for users to explore documentation sections.

In Docusaurus, this is achieved using the `DocCardList` component, which automatically generates cards for all pages within the same directory.

## Example

See the [Community](/community) section for a live example of a Hugo-style index page.

## How to Create a Hugo-Style Index Page

### Step 1: Create or Edit an index.md File

Create an `index.md` file in the directory where you want the category index page. For example, to create a category page for `docs/community/`, create `docs/community/index.md`.

### Step 2: Add the Required Imports

At the top of your markdown file, after the frontmatter, import the `DocCardList` component:

```markdown
---
title: Your Category Title
description: A brief description of this section
sidebar_position: 1
---

import DocCardList from '@theme/DocCardList';
```

### Step 3: Add Content and the DocCardList

Add your introductory content, then include the `DocCardList` component where you want the child pages to appear:

```markdown
## Overview

Add your introductory text here to explain what this section contains.

## Child Pages

<DocCardList />
```

### Step 4: Complete Example

Here's a complete example of a Hugo-style index page:

```markdown
---
title: Community
description: "The greater CNCF Community: TOC and TAGs"
sidebar_position: 1
---

import DocCardList from '@theme/DocCardList';

The CNCF Community is made up of contributors, projects, and organizations 
working together to advance cloud native computing. This section provides 
information about the various groups and initiatives within the CNCF community.

## Community Groups

<DocCardList />
```

## How It Works

The `DocCardList` component automatically:

1. **Scans the directory** - It looks for all markdown files and subdirectories in the same directory as the index.md file
2. **Reads frontmatter** - It extracts the title and description from each file's frontmatter
3. **Generates cards** - It creates clickable cards with the title, description, and a link to each page
4. **Handles nested categories** - Subdirectories with their own index.md files appear as category cards

## Tips and Best Practices

### 1. Use Descriptive Frontmatter

Make sure each child page has clear frontmatter:

```markdown
---
title: A Clear, Descriptive Title
description: A brief description that explains what this page contains
sidebar_position: 1  # Optional: controls the order in the sidebar
---
```

### 2. Customize the Section Heading

You can organize your DocCardList under custom headings:

```markdown
## Getting Started

<DocCardList />

## Advanced Topics

Additional content can go here, or you can have multiple sections.
```

### 3. Add Context Before the Card List

Always provide some introductory text before the DocCardList to give users context about what they'll find in the child pages.

### 4. Sidebar Position

Use the `sidebar_position` frontmatter field to control the order of items:

```markdown
---
title: First Item
sidebar_position: 1
---
```

Lower numbers appear first in both the sidebar and the DocCardList.

## Filtering DocCardList

If you want to show only specific pages (advanced usage), you can filter the items:

```markdown
import DocCardList from '@theme/DocCardList';
import {useCurrentSidebarCategory} from '@docusaurus/theme-common';

export const FilteredDocCardList = () => {
  const category = useCurrentSidebarCategory();
  const filteredItems = category.items.filter(item => 
    item.customProps?.featured === true
  );
  return <DocCardList items={filteredItems} />;
};

<FilteredDocCardList />
```

Note: This requires adding `customProps` to your frontmatter:

```markdown
---
title: Featured Page
customProps:
  featured: true
---
```

## Troubleshooting

### Cards not appearing?

- Ensure child pages have proper frontmatter with at least a `title` field
- Check that files are in the same directory or immediate subdirectories
- Verify the import statement is correct

### Wrong order?

- Use `sidebar_position` in the frontmatter to control ordering
- Lower numbers appear first

### Missing descriptions?

- Add a `description` field to the frontmatter of each child page
- Descriptions appear as subtitle text on the cards

## Related Patterns

- **Category Index Pages**: Use this pattern for any section with multiple child pages
- **Landing Pages**: Combine DocCardList with custom content for rich landing pages
- **Navigation Hubs**: Create navigation hubs by organizing related content under category pages

## See Also

- [Docusaurus DocCardList Documentation](https://docusaurus.io/docs/sidebar/items#embedding-generated-index-in-doc-page)
- [Community Index Page Example](/community)
