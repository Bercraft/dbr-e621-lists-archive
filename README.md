# Danbooru/e621 tag lists archive repo for use in tag autocomplete extensions (+ wildcards and some misc files)

This repo contains mainly through GitHub actions created tag lists of Danbooru and e621.
These tag lists update on a schedule of every 2 months automatically. The script including the workflow making this possible can be found here: https://github.com/DraconicDragon/danbooru-e621-tag-list-processor
All tag lists contain all tags below a post count of 40 (subject to change, first few were 50) and alias tags (both active and deleted, excluding pending from e621)
There are 3 variations:

- danbooru: contains only danbooru tags/aliases
- e621: contains only e621 tags/aliases
- DBRE6: contains a merged list of danbooru and e621 tags/aliases

Note on the DBRE6 merged list: (This should only concern the unrefined merged lists)
In e621, e.g. the tag long_hair is aliased to very_long_hair, while on Danbooru, they are separate tags. This may cause suggestions to show both long_hair and very_long_hair when using very_long_hair and merged list. This shouldn't really cause any issues but it could be a tiny bit confusing or annoying if this somehow bother you.
