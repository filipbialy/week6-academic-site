# Stretch challenges

These are optional. Try them if you finish a checkpoint early.

None of them is needed for the next checkpoint. When the class moves on, you can keep your stretch work in your own copy, or open the next checkpoint folder and carry on with everyone else.

## After checkpoint 01 (semantic HTML)

1. **Validate your pages.** Paste each page into the W3C validator (validator.w3.org/nu) and fix every error.
2. **Use only the keyboard.** Close your mouse hand. Can you reach every link with Tab and follow it with Enter? In which order do the links receive focus?
3. **Check your headings.** List the headings of each page in order (h1, h2, h3). Does the list make sense on its own, as a table of contents?

## After checkpoint 02 (design tokens)

4. **Make your own theme.** Change only the values inside `:root` and give the site a completely different look. You should not need to touch any other rule.
5. **Check the contrast.** Use the WebAIM contrast checker to test each text colour against its background. Normal text needs a ratio of at least 4.5 to 1.

## After checkpoint 03 (layout)

6. **Rewrite with nesting.** Modern CSS lets you put rules inside other rules. Rewrite the `nav` rules so that `nav ul`, `nav a`, `nav a:hover` and the current-page rule all sit inside one `nav { }` block, using `&` where you need it.
7. **Break it on purpose.** Make the browser window very narrow. What goes wrong? Write down each problem. Checkpoint 04 fixes them, so compare your list with what we do next.

## After checkpoint 04 (responsive)

8. **Container queries.** Make each card change its layout based on the width of the card itself, not the screen. Start with `container-type: inline-size` on `.card`, then write an `@container` rule.
9. **Print stylesheet.** Use `@media print` to make the pages print cleanly: no navigation, black text, no background colours, and cards that are not split across two pages.

## After checkpoint 05 (dark mode and accessibility)

10. **Filter publications without JavaScript.** Add three checkboxes (Books, Journal articles, Reports) to the Publications page. Using the `:has()` selector, hide a section when its checkbox is unticked. Next session we will build the same filter with JavaScript, and compare the two.
11. **Page transitions.** Add a smooth transition between pages with `@view-transition { navigation: auto; }`. Which browsers support it? What happens in the others?
12. **Audit the site.** Run Lighthouse (in Chrome DevTools) or the axe browser extension on every page. Fix everything they report and aim for an accessibility score of 100.
