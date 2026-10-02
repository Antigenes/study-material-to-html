# Browser QA for a teaching HTML

Read this when implementing or verifying the HTML artifact. Adapt tools to the available environment; the checks, not a particular browser library, are the requirement.

## Content and source fidelity

1. Check that the source inventory covers every relevant page or slide. Group repeated animation frames under an explained step sequence. Verify displayed page numbers refer to the correct source pages, especially when a PDF's physical page count differs from its printed slide numbers.
2. Compare representative figures at their final displayed size with the originals. Check labels, colour meanings, arrows, formulas, captions, tables, and text inside images. When colours have different meanings in different chapters, explain that difference.
3. Follow worked examples and compute the stated answers. Verify edge cases, assumptions, proof boundaries, and whether time bounds are worst case, expected, or amortized.
4. Check that an apparent correction is supported by the source or by a clear derivation, and is marked as a correction rather than passed off as source wording.

## Offline and browser behaviour

1. Open the final HTML from its local file path or from the packaged offline directory. Verify that no required font, script, image, style, or equation renderer depends on the network.
2. Confirm all images load and can be viewed at useful size. For step-through figures, check the first, middle, and last frames; buttons, slider, caption, counter, and description should stay synchronized.
3. Try chapter links, reveal controls, keyboard focus, image enlargement, font adjustments, and the original-page viewer if present. Check for broken internal links or duplicate IDs.
4. Inspect a desktop viewport and a narrow mobile viewport. Text should remain readable, images retain aspect ratio, code and tables scroll locally if needed, and the whole page should not scroll sideways.
5. Inspect browser console errors. A static HTML parser or script syntax check can catch malformed tags and broken JavaScript before browser QA; it does not replace visual inspection.

Avoid asserting full coverage solely from a matching page count. The lesson text, figures, captions, proofs, and examples must actually convey the source content.
