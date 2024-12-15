## Component Structure

The `Button` component provides various styles and sizes to match different use cases. Below is the structure:

```html
<button class="btn btn-primary btn-md rounded-md">Primary</button>
```

## Classes to Add

### Base Classes

- `btn`: Applies basic button styles, including padding, border radius, and hover/active states.

### Variants

| **Variant**     | **Description**                                                     |
| --------------- | ------------------------------------------------------------------- |
| `btn-primary`   | Styles the button with primary colors.                              |
| `btn-secondary` | Styles the button with secondary colors.                            |
| `btn-outline`   | Adds an outlined style to the button.                               |
| `btn-link`      | Removes background and provides a text button with hover underline. |
| `btn-success`   | Styles the button with success colors (optional).                   |
| `btn-error`     | Styles the button with error colors (optional).                     |

### Size Classes

- `btn-sm`: Applies small padding and font size.
- `btn-medium`: Applies medium padding and font size.
- `btn-lg`: Applies large padding and font size

## Radius Classes for Buttons

| **Class Name**  | **Description**                                       |
| --------------- | ----------------------------------------------------- |
| `.rounded-sm`   | Applies a small border-radius using `--radius-sm`.    |
| `.rounded-md`   | Applies a medium border-radius using `--radius-md`.   |
| `.rounded-lg`   | Applies a large border-radius using `--radius-lg`.    |
| `.rounded-full` | Applies a fully rounded border using `--radius-full`. |
| `.rounded-none` | Removes the border-radius (sets it to `0`).           |

## Accessibility Notes

- **Keyboard Focus**: Buttons are naturally focusable.
- **Disabled State**:
  - Use the `disabled` attribute for non-interactive buttons. The disabled state is styled with reduced opacity and no hover effects.

## Example Usage

### Basic Buttons

```html
<button class="btn btn-primary">Primary</button>
<button class="btn btn-secondary">Secondary</button>
```

### Outline and Disabled

```html
<button class="btn btn-outline">Outline</button>
<button class="btn btn-outline" disabled>Disabled</button>
```

### Text and Rounded

```html
<button class="btn btn-link">Text Button</button>
<button class="btn btn-outline btn-rounded">Rounded</button>
```

### Sizes

```html
<button class="btn btn-primary btn-sm">Small</button>
<button class="btn btn-primary btn-medium">Medium</button>
<button class="btn btn-primary btn-lg">Large</button>
```
