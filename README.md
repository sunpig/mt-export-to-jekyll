# mt-export-to-jekyll

Some [Movable Type](http://www.movabletype.com/) templates for exporting
blog posts and comments to [jekyll](jekyllrb.com/).

## Notes

* Adding the parameter `encode_php="qq"` to entry title and category label handles encoding of
apostrophes, ampersands, and quote marks, as well as html tags in the title and label.
* In the template options for the export entry template, I'm using the following path: 
`jekyll/%y/%y-%m-%d-%-F.html`, which puts the exported posts into a yyyy-year folder below a
top-level `jekyll` directory. Each post is named yyyy-mm-dd-dash-separated-title.html.
* If your entries are in markdown or textile format, use a `.markdown` file
extension. Unfortunately I can't see a way to dynamically set the file extension without
coding up a plugin.

