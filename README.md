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
- This step isn't really necessary. When you test the site, it will generate automatically. I've added it here for completeness.
- `export JEKYLL_VERSION=3.7.3\ndocker run --rm \\n  --volume="$PWD:/srv/jekyll" -p 3000:4000 \\n  -it jekyll/jekyll:$JEKYLL_VERSION \\n  jekyll build`

## Test the Site Locally
1. Install Docker
1. Clone this repository
  - `git clone git@github.com:landrs-toolkit/landrs-toolkit.github.io.git`
1. Change to the repo directory.
  - `cd <repo>`
1. Edit the appropriate content with the text editor of your choice.
1. Serve up the website locally.
  - `export JEKYLL_VERSION=3.7.3\ndocker run --rm \\n  --volume="$PWD:/srv/jekyll" -p 3000:4000 \\n  -it jekyll/jekyll:$JEKYLL_VERSION \\n  jekyll serve`
1. Open a web browser and open the website.
  - [http://localhost:3000](http://localhost:3000)

## Updating Gitlab Pages
- Once all changes are complete and tested, simply commit them back to github on the Master branch.
