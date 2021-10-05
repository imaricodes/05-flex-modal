# A common 'modal' style
This one is another very common pattern on the web. The solution to this one is _simple_... but it might not be immediately obvious to you. You'll need to edit the HTML a bit to get everything where it needs to be.

### a hint
Depending on how to approach this one, you might need to revisit the `flex-shrink` property to keep a flex item from getting smashed.

## Desired outcome

![desired outcome](./desired-outcome.png)

### Self Check

- The blue icon is aligned to the left.
- There is equal space on either side of the icon (the gap between the icon and the edge of the card, and the icon and the text is the same).
- There is padding around the edge of the modal.
- The header, text, and buttons are aligned with each other.
- The header is bold and a slightly larger text-size than the text.
- The close button is vertically aligned with the header, and aligned in the top-right of the card.

Analysis:

I did far too much to get the desired results. Here are my main learning points:

1. Buttons are in-line elements. If written one after another the html, they will appear next to each other on the same line (in-line elements).

2. Each block elements in a sequence will, by default, begin a new line. Or another way to describe this is that they will be stacked vertically.

3. A div inside a flex container becomes an item and will be laid out accordingly.

That's it. If I had kept three two things in mind, I would not have gone to the lenghts (changing the flex direction, unneccsarily wrapping elements in divs, etc.) See more explaination of how my code became so verbose in the html comments.