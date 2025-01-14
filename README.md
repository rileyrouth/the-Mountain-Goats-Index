# Welcome to the Mountain Goats Index!
This site aims to be a comprehensive list of every song, record, and show ever performed by the Mountain Goats. It also includes lyrics, annotations, and lyric changes for as many songs as possible.

We are a fan project run by dedicated amateur volunteers, and are not associated with the band in any way. There's lots of work to do, so feel free to contribute entries to the site! See below for a contribution guide.

## About
The Mountain Goats Index runs on [Jekyll](https://jekyllrb.com) and [Netlify](https://netlify.com).

## Contributing
To contribute pages, simply fork the repository and begin adding files. When you've added as much as you want, create a pull request and I'll look over your contributions.

### Adding Songs
All songs have a default page created automatically from the list in `_data/songs.yaml`. However, in order for a song to have lyrics and other information, a dedicated page needs to be created in the `_songs` folder.[^conflicts] 

A song file should be named after the song with the `.md` extension, and contain the following front matter:

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

### Adding Shows
To add a show, create a file in `_shows` that's named after the date in YYYY-MM-DD format, followed by the venue name, such as `2024-12-10-antones-nightclub.md`. Then, include as much front matter as you can, using this template:

```
---
date: 2012-01-31
city: Charlotte, NC
venue: Visulite Theatre
tour: New Hymns for the Advent of the Serpent God Tour
listen:
  - url: https://archive.org/details/TMG2012-01-31.aud.flac16
    site: Internet Archive
    taper: taperroy
band:
  - John Darnielle
  - Peter Hughes
  - Jon Wurster
banter:
  - quote: "This is a quote I said on stage."
    song: White Cedar
---
```
If any of this front matter isn't relevant (for example, if there's no tape or specific name for the tour), then remove that entire line and any sub-entries.[^removinglisten]

After the front matter (below the final line of three dashes), add the setlist. Only include songs - don't include intros, banter, or other stuff. You can add sections to the setlist by including square brackets around the section title. See below for an example.

```
In Memory of Satan
See America Right
Prowl Great Cain
Song for Lonely Giants
Birth of Serpents
Game Shows Touch our Lives
[Solo]
Commandante
The Day the Aliens Came
You Were Cool
[Band Returns]
White Cedar
Transcendental Youth
Never Quite Free
The Diaz Brothers
Palmcorder Yajna
International Small Arms Traffic Blues
Southwood Plantation Road
[Encore]
The Best Ever Death Metal Band In Denton
No Children
```

### Adding Records
*Coming soon!*

## Other Contributions
I welcome all other contributions, including performance improvements, front-end enhancements, and even features! But please mark these clearly so I can see what's going on - I am still kind of an amateur, so I might need complicated stuff explaining to me before I merge it. But I would still love to see it!

[^conflicts]: This will throw a warning up as Jekyll tries to create two pages with the same name, but seems to be fine as far as I can tell. Welcoming opinions on how best to fix this!

[^removinglisten]: So if there's no tape, you need to remove the lines that start `listen`, `url`, `site`, and `taper`.