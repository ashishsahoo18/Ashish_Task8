# TuteDude MERN Stack – Task: Laundry Services Hamburger Menu in Mobile

## Files Included
- `index.html` — HTML structure
- `style.css` — CSS with Flexbox, Media Queries, and CSS-only hamburger toggle
- `README.md` — This file

## How to Run
1. Unzip the folder.
2. Open `index.html` in Chrome or Firefox.
3. Press F12 → Toggle Device Toolbar → Set width to 375px (Mobile).
4. Click the ☰ hamburger icon to see the menu slide in from the right.

## How the Hamburger Works (No JavaScript!)
The hamburger button is wrapped in a `<button>` tag.
When the button is **clicked/focused**, CSS uses the `:focus` pseudo-class
and the **sibling selector `~`** to show the `.mobile-menu` div:

```css
.hamburger:focus ~ .mobile-menu {
  display: block;
}
```

This works because `.hamburger` and `.mobile-menu` are **siblings** inside `.navbar`.

## Responsive Behaviour

| View    | Width    | Behaviour                                              |
|---------|----------|--------------------------------------------------------|
| Desktop | > 768px  | Full navbar with links, hamburger hidden               |
| Tablet  | ≤ 768px  | Smaller text, links still visible                      |
| Mobile  | ≤ 480px  | Links hidden, hamburger shown, hero in column layout   |

## Requirements Completed
- ✅ Hamburger icon added in navbar — hidden on desktop
- ✅ Hamburger icon visible on mobile only
- ✅ Mobile menu div — position absolute, right side of screen
- ✅ Mobile menu hidden by default (display: none)
- ✅ Menu shows on button focus using `:focus` pseudo-class + `~` sibling selector
- ✅ No JavaScript used
- ✅ No Bootstrap — pure CSS only
- ✅ No inline CSS
- ✅ CSS Variables used

## Submission
1. Put all 3 files in one folder (e.g. `YourName_Task8/`)
2. Compress to `.zip`
3. Rename → `YourName_Task8.zip`
4. Submit on TuteDude portal with deployed link