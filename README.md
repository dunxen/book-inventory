# Shelf scan

Scan the ISBN barcodes on the back of books and get a markdown table of title, author, ISBN and publication date.

Live: https://dunxen.github.io/book-inventory/

- Scans EAN-13 barcodes with the camera ([ZXing](https://github.com/zxing-js/library)); only the 978/979 "Bookland" prefix is accepted, so price add-ons and other barcodes are ignored.
- ISBN-10s typed by hand are validated and converted to ISBN-13.
- Metadata comes from Open Library, falling back to Google Books.
- Every field is editable. The list is kept in `localStorage`.

It's a single static `index.html` with no build step.
