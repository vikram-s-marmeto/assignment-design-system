## **Component Structure**

```html
<div class="card [alignment-class]" tabindex="0" role="region" aria-labelledby="card-title" aria-describedby="card-description">
  <div class="card-image">
    <img src="image-source.jpg" alt="Descriptive image alt text"/>
  </div>
  <h3 class="card-title" id="card-title">Title Text</h3>
  <h4 class="card-subtitle">Subtitle Text</h4>
  <p class="card-description" id="card-description">Description content goes here. It can span multiple lines.</p>
  <a href="link-url" target="_blank" class="btn btn-primary">Call to Action</a>
</div>
```


## Classes to Add

| **Class Name**       | **Description**                                          |
|-----------------------|----------------------------------------------------------|
| `card`               | The main container for the card layout.                  |
| `card-image`         | Wrapper for the image content.                           |
| `card-title`         | The main title of the card.                              |
| `card-subtitle`      | A secondary, descriptive text.                           |
| `card-description`   | Text content to elaborate on the card topic.             |
| `btn`                | A button or link styled as a call-to-action.             |


##  Alignment Classes 

Add the following classes to align content within the `Card` component to parent `.card`:

| Utility Class      | Description                   |
| ------------------ | ----------------------------- |
| `center-content` | Aligns content to the center. |
| `right-content`  | Aligns content to the right.  |
| `left-content`   | Aligns content to the left.   |

### Example Usage:

```html
<!-- Center-Aligned Card -->
<div class="card center-content">
  <h3 class="card-title">Centered Title</h3>
</div>

<!-- Right-Aligned Card -->
<div class="card right-content">
  <h3 class="card-title">Right-Aligned Title</h3>
</div>

<!-- Left-Aligned Card -->
<div class="card left-content">
  <h3 class="card-title">Left-Aligned Title</h3>
</div>
```


## Accessibility Notes

**Keyboard Focus**: The `tabindex="0"` attribute makes the card focusable via keyboard navigation.

- **ARIA Roles**:
  - `role="region"`: Identifies the card as a standalone landmark for assistive technologies.
  - `aria-labelledby`: Links the card to the `id` of its title.
  - `aria-describedby`: Links the card to the `id` of its description for additional context.
