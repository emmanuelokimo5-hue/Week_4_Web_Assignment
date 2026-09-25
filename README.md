# SpendWise Dashboard Shell

## Project Description

SpendWise is a personal finance dashboard designed to give users a clear overview of their spending and financial information.

For Week 4, I transformed my previous Budget Tracker into a modern dashboard shell using CSS Grid and Flexbox.

This version focuses on the visual structure and responsive design. It does not contain JavaScript functionality yet.

## Project Files

### `index.html`

The `index.html` file contains the structure of the SpendWise dashboard.

It includes:

- Sidebar navigation.
- Dashboard header.
- User profile information.
- Financial summary cards.
- Six spending category cards.
- Food category.
- Transport category.
- Rent category.
- Entertainment category.
- Savings category.
- Utilities category.

All financial information is static sample data for this stage of the project.

### `style.css`

The `style.css` file controls the dashboard's appearance and layout.

It includes:

- CSS Grid.
- Flexbox.
- CSS custom properties.
- Responsive design.
- Card styling.
- Sidebar styling.
- Header styling.
- Hover interactions.
- Keyboard focus interactions.
- Dark theme support.

## CSS Grid

CSS Grid is used for the main dashboard layout.

The desktop layout has:

- A 240px sidebar.
- A flexible main content area.

CSS Grid is also used for:

- Financial summary cards.
- Spending category cards.

The category cards are arranged in three columns on larger screens.

## Flexbox

Flexbox is used inside several parts of the dashboard.

It is used for:

- Sidebar navigation.
- Logo section.
- Header.
- User profile.
- Summary cards.
- Category cards.
- Category card content.

Flexbox makes it easier to align and distribute elements.

## CSS Custom Properties

The color theme is defined inside the `:root` selector.

Variables include:

- `--brand-color`
- `--accent-color`
- `--surface-color`
- `--background-color`
- `--primary-text`
- `--secondary-text`
- `--border-color`

These variables are reused throughout the stylesheet to maintain a consistent visual theme.

## Responsive Design

A media query is used at:

```css
@media (max-width: 768px)
```

Below 768px, the dashboard changes to a single-column layout.

The sidebar navigation becomes horizontal and the category cards are displayed in one column.

The responsive layout can be tested using the browser's DevTools Device Toolbar.

## Card Micro-interactions

The spending category cards have hover and keyboard focus effects.

When a user hovers over or focuses on a card:

- The card moves slightly upward.
- The box shadow becomes stronger.
- A focus outline appears for keyboard navigation.

The transition duration is 0.2 seconds, which is 200ms and therefore meets the requirement of 250ms or less.

## Dark Theme

A dark theme has been added as the stretch goal.

It uses:

```css
@media (prefers-color-scheme: dark)
```

Only the CSS custom properties are overridden inside the dark-theme media query.

This allows the dashboard to automatically adapt to a user's system color preference.

## No Absolute Positioning

The dashboard layout does not use absolute positioning.

CSS Grid is used for the overall page structure, while Flexbox is used for arranging elements inside the dashboard.

## Technologies Used

- HTML5
- CSS3
- CSS Grid
- Flexbox
- Google Fonts
- Responsive Design
- CSS Custom Properties

## How to Run

1. Clone or download this repository.
2. Open the project folder.
3. Open `index.html` in a web browser.
4. Use browser DevTools to test the responsive layout.
5. Resize the browser or use the Device Toolbar to check the mobile layout.

## Future Improvements

Future versions of SpendWise can include:

- JavaScript functionality.
- Adding new expenses.
- Removing expenses.
- Calculating total spending.
- Budget tracking.
- Interactive charts.
- Local storage.
- User authentication.
- Dynamic financial reports.
