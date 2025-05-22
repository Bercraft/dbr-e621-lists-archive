# todo: use google bigquery dump in future

### note: the raw mode of my script had an issue where first page it scraped is duplicated, oops

has been fixed but the existing files will have the first page's data duplicated, easy to remove, maybe ill reupload fixed ones at some point

This folder contains the "raw" data from the sites (folder names), not 100% complete because icba with keeping all the data complete, and is mostly so i can look at older tag lists and see if i need them or how things changed i guess, though im probably going to upload *all but the posts* data from now on, so almost 100% complete i guess, either way dont take my word on it and use the google bigquery dump for danbooru or the db export index for e621.

And the above is because i added a "raw mode" to the script mentioned in the root repository, for danbooru at least, which can be found in the ["feat/raw-mode" branch](https://github.com/DraconicDragon/danbooru-e621-tag-list-processor/tree/feat/raw-mode) (merged into main already)

Useful thing: https://huggingface.co/datasets/itterative/danbooru_wikis_full/

the naming is basically (this doesnt apply to the older stuff from 2024 because i didnt bother at the time)

Folder - Year-Month-Day_UTC-TIME

UTC-TIME here meaning the creation date in UTC. For Danbooru creation date means the time at which the script was run while for e621 its the time displayed in [db_export index](https://e621.net/db_export/) (which i assume is UTC, heh)
