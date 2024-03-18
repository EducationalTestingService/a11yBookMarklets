# Prompt for Heading Structure

The following prompts was used to generate the bookmarklet using Claude:

## Step 1

Assume you are an expert in web accessibility, WCAG, javascript, and creating efficient and accessible javascript bookmarklets. I can't write javascript, so I want you to help me. Please create a javascript bookmarklet that analyzes the current web page for the presence of heading elements (H1 to H6), including other elements with a heading role and level, and then create a report in a new window, that is an HTML list structure of the heading levels and the text content of the headings. If there is no heading 1, or multiple heading 1's flag that as a WCAG violation. If heading levels are skipped, i.e., going from heading 1 to heading 3 with out a 2, flag that. Finally, flag any empty headings as errors. Where possible, note the WCAG SC violated for each error. In the report, include the page title, date of report, and page URL.

## Step 2

can you compress the javascript into a single line for efficiency?

### Note

At first, the bookmarklet did not work.  The error recorded in the Chrome Dev Tools was given to Claude, who corrected the code in Step 3

## Step 3

the code crashed and the dev console shows the following error: 2VM38:1 Uncaught TypeError: Assignment to constant variable.

at <anonymous>:1:560

at Array.forEach (<anonymous>)

at <anonymous>:1:193

at <anonymous>:1:1395

### Note

Claude identified the error and corrected the code.