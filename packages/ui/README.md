# @aios/ui

This package provides a comprehensive set of UI components for AIOS applications, based on [shadcn/ui](https://ui.shadcn.com/) and [Tailwind CSS](https://tailwindcss.com/).

## Installation

```bash
npm install @aios/ui
# or
yarn add @aios/ui
```

## Setup

### 1. Configure Tailwind CSS

Include the path to your UI components in your Tailwind configuration:

```js
// tailwind.config.js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    // ...
    "./node_modules/@aios/ui/dist/**/*.{js,mjs}"
  ],
  // ...
}
```

### 2. Import styles

```tsx
// In your root layout or entry file
import "@aios/ui/dist/index.css";
```

## Usage

```tsx
import { Button, Card, Input } from "@aios/ui";

export default function MyComponent() {
  return (
    <Card>
      <Card.Header>
        <Card.Title>Card Title</Card.Title>
        <Card.Description>Card Description</Card.Description>
      </Card.Header>
      <Card.Content>
        <Input placeholder="Enter some text" />
      </Card.Content>
      <Card.Footer>
        <Button>Save</Button>
      </Card.Footer>
    </Card>
  );
}
```

## Available Components

This package includes all components from shadcn/ui:

- Accordion
- Alert
- Alert Dialog
- Aspect Ratio
- Avatar
- Badge
- Button
- Calendar
- Card
- Checkbox
- Collapsible
- Command
- Context Menu
- Dialog
- Dropdown Menu
- Hover Card
- Input
- Label
- Menubar
- Navigation Menu
- Popover
- Progress
- Radio Group
- Scroll Area
- Select
- Separator
- Sheet
- Skeleton
- Slider
- Switch
- Table
- Tabs
- Textarea
- Toast
- Toggle
- Toggle Group
- Tooltip

## License

MIT
