## Configuration
- Site configuration settings are stored in \_config.yaml
- The tagline setting controls the text block on the Home and About pages.

## Pages
- Pages are updated in the \*.md files.
- These are standard markup files.
- Images can be inserted like this:
````
![](/images/DroneDataBuddy/DroneDataBuddyDemo_whitebackground.png)
````
- Links to other pages can be inserted like this:
````
[See more on](/DroneDataBuddy.html)
````

- When creating a new page, add this header to the file:
```
---
layout: page
title: My Page Title
---
```
- Changes are automatically picked up and should appear shortly after commit.

## Posts
- Posts are make by creating a new \*.md file for each post in the \_posts directory.
- The files must be named YYYY-MM-DD-\<Post\>-\<Title\>.md
- When creating a new post, add this header to the file:
```
---
layout: post
title: My Post Title
published: true
---
```
- Setting published to false in the header will cause the post to not be published to the world.
- If the date is in the future, the post will not show up until the correct time.
- Changes are automatically picked up and should appear shortly after commit.

## Test the Site Locally
1. Install Docker
2. Clone this repository
```
git clone git@github.com:landrs-toolkit/landrs-toolkit.github.io.git
```
3. Change to the repo directory.
```
cd <repo>
```
4. Edit the appropriate content with the text editor of your choice.
5. Serve up the website locally.
```
export JEKYLL_VERSION=3.7.3
docker run --rm --volume="$PWD:/srv/jekyll" -p 4000:4000 -it jekyll/jekyll:$JEKYLL_VERSION jekyll serve
```

6. Open a web browser and open the website.
  - [http://localhost:3000](http://localhost:4000)

## Updating Gitlab Pages
- Once all changes are complete and tested, simply commit them back to github on the Master branch.
