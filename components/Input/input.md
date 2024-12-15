### Component Structure

```html
<div class="input-container">
  <label for="name">Name</label>
  <input type="text" id="name" required minlength="3" />
  <p class="input-error">Name must be more than 3 letters</p>
</div>
```

---

### Base Classes

| Class             | Description                                                                                 |
| ----------------- | ------------------------------------------------------------------------------------------- |
| `input-container` | Organizes the input field and label using a flexbox layout with spacing and manages states. |

### Input Styles

| Selector                       | Description                                                               |
| ------------------------------ | ------------------------------------------------------------------------- |
| `input-container label`        | Styles the label with proper font size and weight for clarity.            |
| `input-container input`        | Styles the input field with padding, border-radius, and placeholder size. |
| `input-container .input-error` | Defines the error message with positioning, font size, and error color.   |

### State and Interaction Styles

Add `.input-invalid` `.input-valid` to trigger invalid and valid styles.

| State              | Selector                              | Description                                                                          |
| ------------------ | ------------------------------------- | ------------------------------------------------------------------------------------ |
| **Focus State**    | `input-container input:focus`         | Adds a box-shadow and modifies the border color when the input is focused.           |
| **Invalid State**  | `input-container.input-invalid`       | Marks the input container as invalid and displays the error message.                 |
|                    | `input-container.input-invalid input` | Changes the input border color to error styles.                                      |
|                    | `input-container.input-invalid:focus` | Adds error-specific box-shadow when focused.                                         |
| **Valid State**    | `input-container.input-valid`         | Marks the input container as valid and hides the error message.                      |
|                    | `input-container.input-valid input`   | Changes the input border color to success styles.                                    |
|                    | `input-container.input-valid:focus`   | Adds success-specific box-shadow when focused.                                       |
| **Disabled State** | `input-container:has(input:disabled)` | Applies reduced opacity to the label and input field to indicate the disabled state. |

### Example Usage

#### Invalid State Example

```html
<div class="input-container input-invalid">
  <label for="name">Name</label>
  <input type="text" id="name" required minlength="3" />
  <p class="input-error">Name must be more than 3 letters</p>
</div>
```
