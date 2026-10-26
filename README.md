# Pip's Portfolio: a client revision exercise

## Meet your client

Pip Rummage is a raccoon applying for a job at the Maple Street Lost & Found. Pip is excellent at sorting objects and less excellent at sorting design decisions. They built this resume themselves, named it “Portfolio,” and are very attached to that name. Keep it.

Pip wants the page to feel like a tidy paper resume with a little personality: warm cream, forest green, and a friendly cartoon portrait. Currently, their collection gets more attention than their qualifications. Your job is to carry out the brief below, not rebuild the website from scratch.

The odd styling is intentional. The page starts with working navigation and readable content so you can focus on small, visible improvements.

## Get started

1. Keep all four supplied files in the same folder. Make a copy of the folder if you want a backup.
2. Open `index.html` in a browser (double-click it). Open `index.html` and `style.css` in your editor.
3. Take a “before” screenshot. Read the page and find its matching sections in the HTML.
4. After each small change, save your file and refresh the browser.

### What's in the folder?

| File | Purpose |
| --- | --- |
| `index.html` | Resume content, sections, links, and their order |
| `style.css` | Colors, spacing, fonts, borders, and layout |
| `pip.svg` | The original cartoon portrait; no editing required |
| `README.md` | This client brief and completion checklist |

No JavaScript, installations, accounts, web fonts, or internet connection are needed. The character and work history are fictional. The reserved address `pip@example.com` is a practice address, not a real contact.

## Client change requests

### First, put the content in order

- [ ] **1. Lead with qualifications.** Move the entire “My impressive collection” section to immediately after Education and before Reference. Move the HTML itself; keep all its content and its existing `id`. The final order should be About, Work experience, Skills, Education, Collection, Reference, Contact. Update the small numbered labels so they still run from 01 to 07.
- [ ] **2. Make education easy to find.** Add an Education link to the navigation, between Skills and Contact. It should jump to the existing Education section when clicked.
- [ ] **3. Add one relevant skill.** Add “Inventory record keeping” as a new list item in Skills, using the same HTML element as its neighbors.
- [ ] **4. Make the email useful.** Turn the plain email address into a link using `mailto:pip@example.com`. Keep the visible text `pip@example.com` and the `email` class. Depending on the computer, clicking it may open an email app or ask you to choose one; inspecting the link destination is enough. Do not send an email.

### Then, tidy the design

- [ ] **5. Change the paper and ink.** Change the page background from lavender to warm cream (`#f2eedf`). Change every section heading (`h2`) from pink to forest green (`#315e48`). Keep the pale backgrounds inside the ordinary panels.
- [ ] **6. Retire the novelty heading font.** Give Pip's name the font stack `Arial, sans-serif`, at `42px` on desktop. Keep the supplied narrow-screen rule, which makes it smaller on phones.
- [ ] **7. Let the navigation breathe.** Give each navigation link `18px` of space on its right instead of `2px`. Make sure the links still work and can wrap onto another line in a narrow window.
- [ ] **8. Give the sections room.** Change the inside spacing of every `.panel` from `10px` to `24px`. Keep the outside spacing between sections at `18px`. Be ready to explain the difference between padding and margin.
- [ ] **9. Calm down the portrait.** Replace its pink dashed border with a `3px solid` forest-green border (`#315e48`). Add rounded corners of `16px`. Keep the picture's proportions and its descriptive alternative text.
- [ ] **10. Make the collection less loud.** Give `#collection` the same background (`#fffdf5`) and border (`2px solid #26372e`) as the other panels. Keep it as a separate section. Notice why changing only `.panel` would not fix this section.
- [ ] **11. Make the contact section match.** Align the Contact section's text to the left instead of the right.
- [ ] **12. Give the reference a visual cue.** Add a `4px solid #315e48` left border and `16px` of left padding to the quotation. Keep its existing italic text. Apply the decoration to the quote itself, not the whole Reference panel.

## Stuck? Small hints, not finished code

- A class such as `class="panel"` is selected in CSS with `.panel`. An ID such as `id="contact"` is selected with `#contact`.
- A link to a section uses `href="#section-id"`. The target needs the matching `id`.
- Move a section from its opening `<section ...>` through its matching `</section>`. Indentation helps you see the boundaries.
- A mail link starts its `href` with `mailto:` instead of `https://`.
- Padding is inside the border; margin is outside. Border rounding uses `border-radius`.
- An ID selector is more specific than a class selector. Look for the existing rule that controls an element before adding another rule at the bottom.
- The last block in the CSS is a supplied media query: it applies only when the screen is narrow. You do not need to change it.

## Final checks

- [ ] Refresh the page and compare it with your “before” screenshot.
- [ ] Click every navigation link, the hire button, and Back to top. Each should take you to the right place.
- [ ] Use the Tab key to move through links. Keep the visible keyboard focus outline.
- [ ] Resize your browser to roughly phone width (about 375px). Make sure the content fits without sideways scrolling and the portrait sits above the introduction.
- [ ] Check that you have only one of each section and no repeated IDs after moving content.
- [ ] Create a new GitHub portfolio and host Pip's new resume to help them out.


## Optional challenges

- Style the Skills list as small labels using `display: inline-block`, padding, background color, and rounded corners. Remove the bullets and extra list indentation. Check that the labels wrap on a phone.
- Give the hire button a forest-green background and cream text on hover. Add the same colors for keyboard focus, and keep the focus outline.
- Add a real new resume section called “Volunteer work,” with a heading, a short description, a unique ID, and a matching navigation link. Keep the numbered labels in order.
