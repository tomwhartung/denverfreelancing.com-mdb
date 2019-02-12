
# denverfreelancing.com-mdb

Add Material Design Bootstrap styles to Drew Hornbein's denverfreelancing,com site


# Release Notes

Things to tell Drew when I am close to finishing and ready to deliver the new pages.

- Navigation
  - Links in site menu may need minor updating
    - Using relative file system linking for now, because I'm working with static files (no server)
    - Will probably want to remove the '.' from the './' in the menu href attrs when site goes live with a server
  - Links to external sites menu may need minor updating
    - Had only links to events, not to groups
    - Will need to update for new events, or to a group, as appropriate

# References

- Current site
  - http://denverfreelancing.com/
  - github: https://github.com/dhornbein/denverfreelancing.com/
- MDB
  - https://mdbootstrap.com/


# Plan

For additional context, see `Better_Together_Website-Plan.txt` in this directory.

## Add MDB css and styles to these files:

- index.html
  - Use the full-page-image template
  - https://mdbootstrap.com/previews/free-templates/full-page-image/
- resources.html
  - Use the three-columns-listing template
  - https://mdbootstrap.com/previews/free-templates/three-columns-listing/
- vision.html
  - Use the one-column-listing template
  - https://mdbootstrap.com/previews/free-templates/one-column-listing/


# Process Overview

1. Download MDB template for each page
1.1. Save downloaded file for possible future reference
1.2. Unzip downloaded file into the `Site` directory

2. Remove all unneeded sample freebie templates

3. Merge all three templates under `freebies` into one under `Site`
3.1.

4. Add content from the current site to the template
4.1.

5. Commit completed pages to new branch in Drew's denverfreelancing.com repo
5.1.


## 1. Downloading - Notes

### Download pages

- https://mdbootstrap.com/freebies/jquery/full-background-image/
- https://mdbootstrap.com/freebies/jquery/3-columns-listing/
- https://mdbootstrap.com/freebies/jquery/1-column-listing/

Note: downloaded a file from each of the three pages, but it turns out that
all of them are identical and all contain all freebie templates.

Downloaded file - saved for possible future reference:

- downloaded/Bootstrap-4-templates-master.zip

Unpacked into `freebies` directory.

## 2. Removing unneeded templates - Notes

Removed the following freebie templates from the `freebies` directory:

- admin/
- blog/
- coming-soon/
- e-commerce/
- full-page-image-carousel/
- full-page-video-carousel/
- half-page-image-carousel/
- landing-page/
- magazine/
- portfolio/
- saas/
- two-columns-listing/

Reduced file count by 1350, from 1688 to 338 files.

Note: each of the templates contains mostly identical supporting files.

- Only the style.css and style.scss files differ between freebie templates.

## 3. Merge `freebies` templates into one under `Site`

### Supporting Files: `Site/*`

With one exception - see "(*) Supporting File Exception:" below,
all of the files appearing under each template
are identical, **except index.html** .

We need to start with a single copy of them.

- Starting with supporting files under `freebies/one-column-listing/*`

### (*) Supporting File Exception:

The exception is that the copy of `css/style*.css` in the full-page-image
template, which we are using for the Home, is different from the copy of
`css/style*.css` in the other two templates.

- Home page uses `css/home*.css` instead of `css/style*.css`
  - Source of `css/home*.css` is `freebies/full-page-image/css/style*.css`
- Other pages use `css/style*.css`
  - Note: this file is initially empty

### Home Page: `Site/index.html`

Source:

- full-background-image template: `freebies/full-page-image/index.html`


### Resources Page: `Site/resources.html`

Source:

- 3-columns-listing template: `freebies/three-columns-listing/index.html`


### Vision Page: `Site/vision.html`

Source:

- 1-column-listing template: `freebies/one-column-listing/index.html`




## 4. Adding Content - Notes



## 5. Commiting to new branch in denverfreelancing.com repo



