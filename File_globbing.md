# Matching with *
This challenge introduces use of * glob, we simply use it reference /challenge in under 4 letters by writing cd /ch*, once in the directory we just to run "run" for the flag.
# Matching with ?
This challenge introduces use of ? glob, we simply have follow given instructions to replace a few letters with ? to get the flag.
# Matching with []
This challenge introduces [] glob, we cd into /challenge/files then run the "run" program with argument file_[bash] so it expansion matches the challenge and then get the flag.
# Matching paths with []
Same as last challenge but this time we use the path as an argument using [] glob to get the flag, /challenge/run /challenge/files/file_[bash].
# Mixing globs
Since this challenge required to find the matching files from a bunch of given names, I first used ls -a to see all files present in the directory, for my attempt I used ?[wdh]* to match challenging, educational, pwing but this also matched the file "thrilling" so I tried to think of another pattern to match these 3 words, I started to think how to unmatch the word thrilling but after spending 20 mins I could not figure out a way to do so. So instead of finding pattern between these 3 words I looked at all the file names present and tried to find a pattern from there, here it became obvious very quick that only 3 words start with c, e and p so the matching pattern would be [cep]*. I checked with ls [cep]* and found the solution to be correct yet couldnt get the flag. I tried /challenge/run [cep]* and finally got the flag, this challenge didn't mention this step somehow so I thought the way to get final flag might be different but it was not.
# Exclusionary globbing
Similar to the last challenge but instead of finding files that start with specific names we find the files not starting with specified letters by using ! or ^, the expression being [^pwn]* and we get the flag.