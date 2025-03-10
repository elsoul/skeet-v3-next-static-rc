---
id: building-your-application-worker-cron
title: Deploy Cron Worker
description: Deploy Cron Worker Skeet Framework
---

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

**Bold Text**

_Italic Text_

~Strikethrough Text~

- Unordered List Item 1
- Unordered List Item 2
  - Nested Unordered List Item 1
  - Nested Unordered List Item 2

1. Ordered List Item 1
2. Ordered List Item 2
   1. Nested Ordered List Item 1
   2. Nested Ordered List Item 2

Testing `Inline code snippet` like this.

```javascript
// Code block
console.log('Hello, World!')
```

---

## Code Sample

```tsx:/src/app/[locale]/(default)/layout.tsx

import { setRequestLocale } from 'next-intl/server'
import DefaultHeader from './DefaultHeader'
import DefaultFooter from './DefaultFooter'

type Props = {
  children: React.ReactNode
  params: {
    locale: string
  }
}

export default async function DefaultLayout({
  children,
  params: { locale },
}: Props) {
  setRequestLocale(locale)

  return (
    <>
      <div className="flex flex-col">
        <DefaultHeader />
        <main className="min-h-screen">{children}</main>
        <DefaultFooter />
      </div>
    </>
  )
}

```

## YouTube Embed

https://www.youtube.com/watch?v=t4KHXqguTi8
