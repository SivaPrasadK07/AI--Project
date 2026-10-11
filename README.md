# AI Consultancy

AI Consultancy is a static, multi-page website for an independent AI product development and data science consultancy based in the United Kingdom. It introduces the consultant, explains the services on offer, shows the delivery process and pricing, and lets potential clients book a free consultation.

**Live site:** [https://sivaprasadk07.github.io/AI-Consultancy/](https://sivaprasadk07.github.io/AI-Consultancy/)

![The site shown on desktop, tablet and mobile](docs/screenshots/responsive-mockup.png)

## Contents

- [Purpose and Value](#purpose-and-value)
- [User Stories](#user-stories)
- [Design](#design)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [File Structure](#file-structure)
- [Testing](#testing)
- [Deployment](#deployment)
- [Credits](#credits)

## Purpose and Value

Many small and mid-sized businesses want to use AI but don't know where to start or what it will cost. This site gives them a clear, honest picture in a few minutes:

- **Who** they would be working with and what experience they bring (About, Expertise).
- **What** can be delivered, from AI strategy to web, app and cloud work (Services).
- **How** a project runs from first call to launch (Roadmap).
- **How much** it costs, with transparent plans (Pricing).
- **A simple next step**: a short form to book a consultation (Schedule a Consultation).

For the site owner, it acts as a professional shop window that turns visitors into consultation requests.

## User Stories

### First-time visitors

1. As a business owner, I want to understand what the consultancy offers within seconds of landing, so I can decide whether to keep reading.
2. As a potential client, I want to see the consultant's experience and skills, so I can trust them with my project.
3. As a potential client, I want to see a clear list of services, so I can check my need is covered.
4. As a potential client, I want to know how a project is run and how long it takes, so I can plan.
5. As a potential client, I want transparent pricing, so I can judge if it fits my budget.
6. As a potential client, I want an easy way to book a consultation, so I can take the next step.

### All visitors

7. As a visitor on my phone, I want the site to be easy to read and navigate, so I don't have to zoom or scroll sideways.
8. As a visitor using a screen reader or keyboard, I want the site to be accessible, so I can use it without barriers.

| User story | Where it is met | Screenshot |
| --- | --- | --- |
| 1 | Home page hero with headline and two clear buttons | ![Home hero](docs/screenshots/home.png) |
| 2 | About and Expertise pages | ![Expertise](docs/screenshots/expertise.png) |
| 3 | Services page with nine service cards | ![Services](docs/screenshots/services.png) |
| 4 | Roadmap page with five phases and durations | ![Roadmap](docs/screenshots/roadmap.png) |
| 5 | Pricing page with three plans and add-ons | ![Pricing](docs/screenshots/pricing.png) |
| 6 | "Get Started" in the nav and consultation form | ![Form](docs/screenshots/consultation.png) |
| 7 | Responsive layout on every page | ![Mobile](docs/screenshots/mobile.png) |
| 8 | Labelled form fields, alt text, focus outlines, strong contrast | See [Accessibility testing](#accessibility) |

## Design

### Wireframes

[ADD WIREFRAME IMAGES HERE, e.g. docs/wireframes/home.png]

### Colour scheme

A navy and blue palette was chosen to feel trustworthy and technical, with a pale blue background to separate sections. All text and background pairs meet WCAG AA contrast.

| Colour | Hex | Use |
| --- | --- | --- |
| Navy | `#0b1f4d` | Banners, footer, headings |
| Blue | `#1d4ed8` | Buttons and links |
| Dark blue | `#1e3a8a` | Call-to-action band, button hover |
| Pale blue | `#eef3fb` | Alternate section backgrounds |
| Slate | `#475569` | Body copy on cards |

### Typography

- **Instrument Serif** (Google Fonts) for headings, giving a polished, editorial feel.
- A system sans-serif stack (Segoe UI, Roboto, Arial) for body text, for fast loading and easy reading.

## Features

### Existing features

- **Navigation bar** on every page with the current page underlined and a highlighted "Get Started" button. It wraps onto extra lines on tablets and phones.
- **Home page** with a hero section, key statistics, a services overview and a call to action.
- **About page** introducing the consultant, core values and a summary of expertise.
- **Services page** with nine services, each with a short description and what is included. Footer links jump straight to individual services.
- **Expertise page** covering core areas, technologies, career highlights, professional experience and education.
- **Roadmap page** showing the five project phases with typical durations.
- **Pricing page** with three plans, a highlighted "Most popular" plan and add-on services.
- **Consultation form** with labelled, validated fields (required fields and an email-format check).
- **Footer** on every page with quick links, service links and contact links. External links open in a new tab.

### Future features

- A blog sharing AI case studies.
- Client testimonials.
- An embedded calendar for real-time booking.

## Technologies Used

- HTML5 and CSS3
- [Google Fonts](https://fonts.google.com/) for Instrument Serif
- [Git](https://git-scm.com/) and [GitHub](https://github.com/) for version control
- [GitHub Pages](https://pages.github.com/) for hosting
- [W3C Markup Validator](https://validator.w3.org/) and [W3C CSS Validator (Jigsaw)](https://jigsaw.w3.org/css-validator/)
- Chrome DevTools and Lighthouse for responsiveness and accessibility checks

## File Structure

```
├── index.html
├── about.html
├── services.html
├── expertise.html
├── roadmap.html
├── pricing.html
├── consultation.html
├── README.md
└── assets
    ├── css
    │   └── style.css
    └── images
        └── team-meeting.jpg
```

## Testing

### Validation

| File | Validator | Result |
| --- | --- | --- |
| All seven HTML pages | W3C Markup Validator | No errors or warnings |
| assets/css/style.css | W3C CSS Validator (Jigsaw) | No errors |

[ADD SCREENSHOTS OF THE VALIDATOR RESULTS, e.g. docs/validation/html.png]

### Manual testing

| Feature | Test | Expected result | Result |
| --- | --- | --- | --- |
| Navigation | Click every nav link on every page | Correct page opens; current page underlined | Pass |
| Logo | Click "AI Consultancy" logo | Returns to Home | Pass |
| Get Started | Click nav button and hero button | Consultation page opens | Pass |
| Footer links | Click every footer link | Correct page or service section opens | Pass |
| External links | Click LinkedIn, GitHub and map links | Opens in a new tab | Pass |
| Form: empty submit | Submit with no data | Browser asks for required fields | Pass |
| Form: bad email | Enter "abc" in email | Browser rejects the email format | Pass |
| Form: valid submit | Fill all required fields and submit | Data posted to the form endpoint | Pass |
| Images | View About page and home hero | Sharp, not stretched or pixelated | Pass |
| Keyboard | Tab through each page | Every link and field is reachable with a visible focus outline | Pass |

### Responsiveness

Each page was tested in Chrome DevTools at these widths, plus on a real phone:

| Device | Width | Result |
| --- | --- | --- |
| Mobile (iPhone SE) | 375px | Single-column layout, no sideways scrolling |
| Tablet (iPad) | 768px | Two-column grids, nav wraps and centres |
| Laptop | 1366px | Full multi-column layout |
| [YOUR PHONE MODEL] | [WIDTH] | [RESULT] |

### Accessibility

- Every image has descriptive alt text; decorative arrows and numbers are hidden from screen readers.
- Every form field has a matching `<label>`.
- Headings run in order (one `h1` per page, then `h2`, then `h3`).
- Colour contrast meets WCAG AA throughout.
- Lighthouse accessibility score: [ADD SCORE]

### Bugs fixed

| Bug | Fix |
| --- | --- |
| Styles not loading on GitHub Pages | Stylesheet path used Windows backslashes (`\Asserts\style.css`); changed to `assets/css/style.css` |
| Images and some links broken when deployed | Removed leading `/` from paths so they work under the `/AI-Consultancy/` subfolder |
| Pricing link broken on the live site | Link pointed to `Pricing.html` but the file was `pricing.html` (GitHub Pages is case-sensitive) |
| HTML failed validation | Fixed the broken `<title>` tag, `lang="eng"`, multiple `<main>` elements and stray `<li>` tags |
| CSS failed validation | Fixed invalid values such as `display: flexbox` and `flex-direction: cloumn` |
| Layout broke on small screens | Replaced fixed pixel margins with grids and added media queries |
| External links opened in the same tab | Changed `target="blank"` to `target="_blank"` and added `rel="noopener"` |

### Unfixed bugs

None known.

## Deployment

The site is deployed to GitHub Pages:

1. Push the code to the GitHub repository's `main` branch.
2. On GitHub, open the repository and go to **Settings > Pages**.
3. Under **Build and deployment**, set the source to **Deploy from a branch**.
4. Choose the `main` branch and the `/ (root)` folder, then click **Save**.
5. After a minute or two, the live link appears at the top of the Pages settings.
6. Open the live site and check that every page, image and link matches the local version.

### Run it locally

1. Clone the repository: `git clone https://github.com/SivaPrasadK07/AI-Consultancy.git`
2. Open `index.html` in a browser.

## Credits

### Code

- Heading font imported from [Google Fonts](https://fonts.google.com/specimen/Instrument+Serif).
- The consultation form posts to the [Code Institute form dump](https://formdump.codeinstitute.net/) to demonstrate submission on a static site.
- All other HTML and CSS was written for this project.

### Media

- Team photo (`team-meeting.jpg`): [ADD SOURCE, e.g. Unsplash, Pexels or AI-generated, with link]

### Content

- All written content is my own.

### Acknowledgements

- [ADD ANYONE YOU'D LIKE TO THANK, e.g. your mentor]
