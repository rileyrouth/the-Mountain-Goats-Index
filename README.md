# Welcome to the Mountain Goats Index!
This site aims to be a comprehensive list of every song, record, and show ever performed by the Mountain Goats. It also includes lyrics, annotations, and lyric changes for as many songs as possible.

We are a fan project run by dedicated amateur volunteers, and are not associated with the band in any way. There's lots of work to do, so feel free to contribute entries to the site! See below for a contribution guide.

## About
The Mountain Goats Index runs with [Jekyll](https://jekyllrb.com) and [Netlify](https://netlify.com).

## Contributing
To contribute pages, simply fork the repository and begin adding files. When you've added as much as you want, create a pull request and I'll look over your contributions.

### Adding Songs
All songs have a default page created automatically from the list in `_data/songs.yaml`. However, in order for a song to have lyrics and other information, a dedicated page needs to be created in the `_songs` folder.[^conflicts]

A song file should be named after the song, and contain the following front matter:

```
---
title: Lakeside View Apartments Suite
---
```

After that, fill in the lyrics, making sure to add the necessary `\\` after each line that doesn't end a verse. (Look at any existing song to see what I mean.)

You can add annotations to lyrics by including the footnote symbol: `[^footnotename]`, ensuring each footnote in the page has a unique name (i.e. `[^lakesidelocation]` or `[^portland]`). Then, at the bottom of the page, repeat that footnote name and a colon, then write your footnote:

```
[^lakesidelocation]: No specific suite of apartments exists in the specified area with this name, as far as I can see.
```

[^conflicts]: This will throw a warning up as Jekyll tries to create two pages with the same name, but seems to be fine as far as I can tell. Welcoming opinions on how best to fix this!
