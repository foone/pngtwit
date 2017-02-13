# pngtwit
A tool to help you post PNGs to twitter without quality loss

Twitter assumes any PNG you're posting is because you don't understand image formats, so it "helpfully" converts them to JPEGs for you. But if you do understand image formats and were just trying to post some clean pixel art, this is a problem.

pngtwit is here to help. It provides several methods to get around twitter's JPEGification:

* Extra-row: Add an extra row of transparent pixels at the bottom of the image
* Extra-column: Same as extra-row, but with a column of transparent pixels instead of a row
* Transparent-border: Add a transparent 1-pixel border on all sides
* Single-pixel: Mark the bottom-right pixel transparent. Good for screenshots!
* Stealth-pixel: Make the bottom-right pixel 0.4% transparent. Invisible to humans, obvious to Twitter.

When run without options, automatically applies the default method to the selected image, unless the image would already be safe.
You can configure which method is chosen by default with a .pngtwitrc file. 
