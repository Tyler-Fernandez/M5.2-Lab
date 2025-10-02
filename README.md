# web-dev-starter

This is a starter project for web development with no frameworks and minimal
dependencies. It is intended to be a starting point for web development projects
that are written in plain HTML, CSS, and JavaScript.

## Getting Started

To get started, clone this repository and run the following commands:

```bash
npm install
```
This will install the necessary dependencies for the project.

## Development

It is recommended to use the VSCode Live Server extension to run the project
locally. This will allow you to see changes in real-time as you make them. There
is no need to run a build process or refresh the page manually. Additionally,
you do not need to setup a local server to run the project.

## Testing

To run the tests for the project, run the following command:

```bash
npm test
```

# Accessibility Lab Answers

## Color
When put into WebAIM's color contrast checker, the current color scheme fails for normal text and only passes 1 text for large text.

## Semantic HTML
When using a screenreader, you can't jump between headings and it's hard to tell where headings and paragraphs start and end. To make the article text easier for screenreader users to navigate, br tags need to be removed, font tags replaced with heading elements, and paragraphs wrapped with p. The navigation part of the site can be wrapped with the nav tag.

## The images

Fixed by using aria-labelledby.

## The audio player
A link to a separate file is added for hearing impaired people and to make the audio accessible to older browsers.
## The forms

To add a label accessible to only screenreaders, add a label to aria-label on the input element. To make the label texts associated with their labels, the label text needs to be wrapped with label elements with for attributes containing hte ID values of the input elements.
</dl>

## The show/hide comment control

Can be fixed by changing the div to a button element.

## The table

The table is now within a summary attribute, each cell in the first row and column uses th, and the scope for rows in the first column is scope="row" and the scope for columns in the first row is scope="col".


## Other considerations
To make the site more accessible, adding media queries would make it more accessible on mobile devices. Additionally, client-side validation could be added to the comment form.
