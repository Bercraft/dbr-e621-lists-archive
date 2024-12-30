### experimental, probably inaccurate wildcard list. **a lot of testing needed**.

## Found false positives? - create a GitHub issue here or on the script repo or tell me on CivitAI.com/user/DraconicDragon or Discord @i.eat.plutonium (I'm also on the CivitAI Discord server)

contents are characters (danbooru only for now), 1 tag per line, filtered by gender in 3 text files, no underscore, backslashes before brackets

#### the full list (like post count threshold 8) is very inaccurated to the bottom because theres tags there that may have like 10 posts but they are all 403 forbidden

## also i really need to save these as csv 🙃 with post count column some stuff is easier, and i can save all genders in one file with gender column
coming soon:tm:

why not androgynous but indeterminate? - because its almost impossible to identify androgynous reliably and theres a lot of tags in indeterminate that are literally indeterminate because it wasnt possible to determine them accurately

its possible to match similar spelled tags but often that is not the case and i dont know if theres a gender change with them and i cant exactly check that really reliably either (less chance of false positive than androgynous but still a pain to filter)

first pass is using simple filtering method and second pass is implications filtered from indeterminate into male/female like saber \(fate\) is matched with artoria pendragon \(fate\) into female tags because saber implicates artoria pendragon

this is done because first pass ignores posts with 2 characters and saber is ALWAYS artoria pendragon but artoria is not always saber and the script skips any post with more than 1 character tags, so saber cant get identified in first pass

i found it easier to make a second pass filter for this that filters implications correctly and moves character_name_(female) from indeterminate (since its also implication often) to their respective file
