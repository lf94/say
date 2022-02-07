```
#!/bin/sh
#
# Say - a simple, opinionated speech script.
# Dependencies: espeak-ng, mbrola, mbrola-us*
# 
# Usage: say "some text"
#
# I typically use it when something is done, so that I don't need to watch
# any processes and just use my hearing instead:
#
# npx webpack && npm pack dist/ && say done
#
# It can then be used in editors like vim or kakoune for other audio cues, or
# chat clients like weechat to read private messages.
#

echo "$1" | espeak-ng -v english-mb-en1 -p 80 -s 145 --punct="|"

```
