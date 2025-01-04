#### Folders
57swap_exp is the same as old_cat_merge but with e6 categories 5 and 7 swapped - created because of an anonymous suggestion

old_cat_merge contains files that were simply merged together without regards to the category number so dbr's meta tags are merged together with e6's species tags

The files in this folder are newer and separate e6 and dbr categories without merging unrelated categories by starting e6 tags at 7 and going up from there.

#### Filename info
pt2 / pt25 / pt50 = post threshold
ia = includes 'active' aliases 
dd = includes danbooru deleted aliases
ed = includes e621 deleted aliases
ep = includes e621 pending aliases (unlikely to appear)

#### Merged lists info

**CONTRIBUTOR (9) is new!** See https://e621.net/forum_topics/54179 
Tag lists *before 18th december* will have copyright instead of contributor in the same category slot. For AI related things this category and it's tags can very likely be ignored

| Value	| Description | Site |
|-------|-------------|------|
|0	    | General     | danbooru |
|1	    | Artist      | danbooru |
|2	    | Invalid     |  |
|3	    | Copyright   | danbooru |
|4	    | Character   | danbooru |
|5	    | Meta        | danbooru |
|       |             |          |
|6	    | Invalid     |  |
|7	    | General     | e621 |
|8	    | Artist      | e621 |
|9	    | Contributor | e621 |
|10	    | Copyright   | e621 |
|11	    | Character   | e621 |
|12	    | Species     | e621 |
|13	    | Invalid     |  |
|14	    | Meta        | e621 |
|15	    | Lore        | e621 |

Categories 2, 6 and 13 shouldn't have any tags associated with them

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
    "6": ["red", "maroon"],
    "7": ["lightblue", "dodgerblue"],
    "8": ["gold", "goldenrod"],
    "9": ["gold", "goldenrod"],
    "10": ["violet", "darkorchid"],
    "11": ["lightgreen", "darkgreen"],
    "12": ["tomato", "darksalmon"],
    "14": ["whitesmoke", "black"],
    "15": ["seagreen", "darkseagreen"]
}
```
Remove 9 from the json if you are using a merged tag list from before december 18th and subtract 1 from anything 10 or above to get the right colors