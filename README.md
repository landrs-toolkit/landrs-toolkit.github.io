## Pages
- Pages are updated in the \*.md files.
- These are standard markup files.

## Posts
- Posts are make by creating a new \*.md file for each post in the \_posts diretory.
- The files must be named YYYY-MM-DD-\<Post\>-\<Title\>.md

## Generating the Static Pages
`export JEKYLL_VERSION=3.7.3\ndocker run --rm \\n  --volume="$PWD:/srv/jekyll" -p 3000:4000 \\n  -it jekyll/jekyll:$JEKYLL_VERSION \\n  jekyll build`

## Test Locally
`export JEKYLL_VERSION=3.7.3\ndocker run --rm \\n  --volume="$PWD:/srv/jekyll" -p 3000:4000 \\n  -it jekyll/jekyll:$JEKYLL_VERSION \\n  jekyll serve`
