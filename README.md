# mit-license
to get a link to mit license raw text
 ```bash
 curl -sL 'https://raw.githubusercontent.com/ccdd13/mit-license/main/mit-template.txt' | \
 sed  -Ee "s~\\[year\\]~$(date '+%Y')~ig;s~\\[fullname\\]~$(echo -n ${GITHUB_ACTOR})~ig" \
            > LICENSE.txt
 
 ```
