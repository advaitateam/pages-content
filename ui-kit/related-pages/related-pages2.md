---
layout: uikit-single
title: Related Pages 2
slug: related-pages-2
draft: true
publishDate: 2024-10-10
tags:
  - ui-kit
---

The `VRelatedPages` component is a Vue 3 component that displays a table of related pages, grouped by a specified category.

## Props
| Prop Name   | Type                      | Required | Description |
|-------------|---------------------------|----------|-------------|
| `data`      | `IRelatedPages[]`        | Yes      | An array of related pages, each containing a group and its items. |

``` ts
interface IRelatedPages {
    groupBy: IFrontmatter;
    items: IFrontmatter[];
}
```

## Example
```vue
<script setup lang="ts">
import VRelatedPages from '@/components/common/VRelatedPages.vue';
  const items = [
        { title: 'Related Page 1', url: '/related-page-1' },
        { title: 'Related Page 2', url: '/related-page-2' },
      ]
</script>
<VRelatedPages :items="items" />
```


<script setup lang="ts">
import VRelatedPages from '@/components/common/VRelatedPages.vue';
  const items = [
        { title: 'Related Page 1', url: '/related-page-1' },
        { title: 'Related Page 2', url: '/related-page-2' },
      ]
</script>
<VRelatedPages
            sub-title="Последние события"
            :items="items"
          />
