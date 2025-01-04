57swap_exp is the same as old_cat_merge but with e6 categories 5 and 7 swapped - created because of an anonymous suggestion

old_cat_merge contains files that were simply merged together without regards to the category number so dbr's meta tags are merged together with e6's species tags

The files in this folder are newer and separate e6 and dbr categories without merging unrelated categories by starting e6 tags at 7 and going up from there.

| Value	| Description | site |
|-------|-------------|------|
|0	    | General     | danbooru |
|1	    | Artist      | danbooru |
|3	    | Copyright   | danbooru |
|4	    | Character   | danbooru |
|5	    | Meta        | danbooru |
|
|6	    | Invalid     | e621 |
|7	    | General     | e621 |
|8	    | Artist      | e621 |
|9	    | Copyright   | e621 |
|10	    | Character   | e621 |
|11	    | Species     | e621 |
|12	    | Invalid     | e621 |
|13	    | Meta        | e621 |
|14	    | Lore        | e621 |

e621 tags that already exist in danbooru like solo have been merged into the danbooru categories since these csvs are still autocomplete focused, if you want pure e621, visit the e621 folder.

### for sd-webui-tagcomplete use this color config json and rename file to danbooru_e621.csv

You can also change the key's name in the json to match whatever name the csv file has.

```json
"danbooru_e621": {
    "-1": ["red", "maroon"],
    "0": ["lightblue", "dodgerblue"],
    "1": ["indianred", "firebrick"],
    "3": ["violet", "darkorchid"],
    "4": ["lightgreen", "darkgreen"],
    "5": ["orange", "darkorange"],
    "7": ["lightblue", "dodgerblue"],
    "8": ["gold", "goldenrod"],
    "10": ["violet", "darkorchid"],
    "11": ["lightgreen", "darkgreen"],
    "12": ["tomato", "darksalmon"],
    "14": ["whitesmoke", "black"],
    "15": ["seagreen", "darkseagreen"]
}
```