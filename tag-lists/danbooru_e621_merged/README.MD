#### Folders

The files in this folder level are 'newer' compared to the ones in "unrefined_aliases" and separate e6 and dbr categories without merging unrelated categories by starting e6 tags at 7 and going up from there. These files also include an updated treatment where every alias that already exists exactly as a normal tag was deleted. (comfyui custom scripts will redirect to the wrong tag otherwise, the a1111 sd tagcomplete extension doesnt have this issue)

- unrefined_aliases contains folders/files that did not get the updated treatment of removing aliases if they already existed as normal tags.

- 57swap_exp is the same as old_cat_merge but with e6 categories 5 and 7 swapped - created because of an anonymous suggestion

- old_cat_merge contains files that were simply merged together without regards to the category number so dbr's meta tags are merged together with e6's species tags

#### Filename info

pt2 / pt25 / pt50 = post count threshold

ia = includes 'active' aliases

dd = includes danbooru deleted aliases

ed = includes e621 deleted aliases

ep = includes e621 pending aliases (unlikely to appear)

dpc / epc / spc = merged post count type:

- dpc = post count value taken from danbooru
- epc = value taken from e621
- spc = value is the sum of both danbooru + e621

anything after the above suffixes is some extra info if needed. For example "_sum" means the post count is a sum of both (default settings was that the post count value would be taken from the danbooru list); subject to change

#### Merged lists info

**CONTRIBUTOR (9) is "new"** See <https://e621.net/forum_topics/54179>
Tag lists *before 18th december 2024* will not have this category in the CSV files. For AI related things this category and it's tags can very likely be ignored, and even deleted i guess, but they are still in there, might be gone in the future though (the script will be updated accordingly).

| Value | Description | Site     |
|-------|-------------|----------|
|0      | General     | danbooru |
|1      | Artist      | danbooru |
|2      | *Invalid*   |          |
|3      | Copyright   | danbooru |
|4      | Character   | danbooru |
|5      | Meta        | danbooru |
|       |             |          |
|6      | *Invalid*   |          |
|7      | General     | e621     |
|8      | Artist      | e621     |
|9      | Contributor | e621     |
|10     | Copyright   | e621     |
|11     | Character   | e621     |
|12     | Species     | e621     |
|13     | *Invalid*   |          |
|14     | Meta        | e621     |
|15     | Lore        | e621     |

Categories that show "*Invalid*" don't show up in the tag lists and don't have any tags associated with them

e621 tags that already exist in danbooru like solo have been merged into the danbooru categories since these csvs are still autocomplete focused, if you want pure e621, visit the e621 folder, the same goes for danbooru of course.

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
