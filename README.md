## Pages
- Pages are updated in the \*.md files.
- These are standard markup files.
- Changes are automatically picked up and should appear shortly after commit.

## Posts
- Posts are make by creating a new \*.md file for each post in the \_posts directory.
- The files must be named YYYY-MM-DD-\<Post\>-\<Title\>.md
- If the date is in the future, the post will not show up until the correct time.
- Changes are automatically picked up and should appear shortly after commit.

## Generating the Static Pages Locally
`export JEKYLL_VERSION=3.7.3\ndocker run --rm \\n  --volume="$PWD:/srv/jekyll" -p 3000:4000 \\n  -it jekyll/jekyll:$JEKYLL_VERSION \\n  jekyll build`

## Test the Site Locally
`export JEKYLL_VERSION=3.7.3\ndocker run --rm \\n  --volume="$PWD:/srv/jekyll" -p 3000:4000 \\n  -it jekyll/jekyll:$JEKYLL_VERSION \\n  jekyll serve`
