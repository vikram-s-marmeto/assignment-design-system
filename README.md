# Design System Documentation

## Overview

This design system provides a set of highly crafted, reusable UI components that are modular, scalable, and consistent across web applications. The system is built with a focus on flexibility, ease of customization, and maintainability.

## Table of Contents

- [Introduction](#introduction)
- [Reset CSS and Global Styles](#reset-css-and-global-styles)
- [Color System](#color-system)
- [Typography](#typography)
- [Spacing](#spacing)
- [Component Structure](#component-structure)
- [State Management](#state-management)
- [Example Usage](#example-usage)

## Introduction

Our design system follows modern best practices to ensure ease of use and maintainability. The core principles are based on:

- **Consistency**: The design system ensures consistent UI components across your application.
- **Flexibility**: The system is customizable with CSS variables.

```plaintext
assets/
components/
  └── button/
      ├── button.html
      └── button.css
css/
  ├── reset.css
  ├── spacing.css
  ├── colors.css
  ├── typography.css
  └── utils.css
layout/
index.html
```

## Folder structure

| **Folder**    | **Description**                                                                                                  |
| ------------- | ---------------------------------------------------------------------------------------------------------------- |
| `assets/`     | Contains assets like images, icons, or other media files used in the design system.                              |
| `components/` | Contains individual components used in the design system, each with its own HTML and CSS files for easy copying. |
| `css/`        | Stores global CSS files, including reset, spacing, typography, colors, and utility classes.                      |
| `layout/`     | Holds common layout HTML templates shared across all pages, including headers, footers, etc.                     |
| `index.html`  | The main entry HTML file that links all global styles, components, and layouts.                                  |

## Reset CSS and Global Styles

To ensure consistency across browsers, we used the `:where()` pseudo-class in our reset CSS. This allows us to apply global styles while keeping specificity low, ensuring that the component styles do not conflict with any other custom styles.

## Color System

The color system uses CSS variables to maintain consistency across the UI. Variables allow for easy customization of primary, secondary, background, text, and error colors, which can be adjusted globally.

### Example Color Variables:

```css
:root {
  --primary-color: #3498db;
  --secondary-color: #2ecc71;
  --error-color: #e74c3c;
  --background-color: #ffffff;
  --text-color: #333333;
}
```

## Typography

The typography system uses variables for font sizes, font families, and font weights to ensure consistency. This allows you to easily adjust the typography across the entire application.

### Example Typography Variables:

```css
:root {
  --text-xs: 12px;
  --text-sm: 14px;
  --text-md: 16px;
  --text-lg: 18px;
}
```

## Spacing

Spacing is also managed using CSS variables for margins, paddings, and gap spacing. This makes layout adjustments simple and ensures consistent spacing throughout the application.

### Example Spacing Variables:

```css
:root {
  --spacing-xxs: 4px;
  --spacing-xs: 8px;
  --spacing-sm: 12px;
  --spacing-md: 16px;
  --spacing-lg: 24px;
  --spacing-xl: 32px;
  --spacing-xxl: 48px;
}
```

### Component Documentation

The documentation for each component can be found in its respective folder under the `components/` directory.

- [Button Component](./components/Button/button.md)
- [Card Component](./components/Card/card.md)
- [Input Component](./components/Input/input.md)
