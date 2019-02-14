
# denverfreelancing.com-mdb

Add Material Design Bootstrap styles to Drew Hornbein's denverfreelancing,com site


# Release Notes

Things to tell Drew when I am close to finishing and ready to deliver the new pages.

- General
  - I considered using "Front Range Freelancing" instead of "Denver Area Freelancing" in the "logo" in the header
  - "Front Range Freelancing" is alliterative and a little bit shorter
  - Also, I sense you want to be more inclusive than exclusive
  - Just a thought...
- Favicon: took a screenshot of the font awesome globe icon and reduced it to 32x32
- Navigation
  - The logo "Denver Area Freelancers" and Home menu options are redundant
  - Moved email subscription signup form to its own page
    - Added an option for it to the main menu
  - Links to meetup and facebook on the right side of the menu may need minor updating
    - Had only links to events, not to groups
    - Note: Will need to update for new events, or to a group, as appropriate
- Home Page
  - Moved email list signup form to a separate page
- Vision Page
  - There are ways to lighten or darken the image, and adjust the text accordingly to make the text more readable
- Resources Page
  - If you want an affiliate link disclosure, a full page with details, I can adjust the one I wrote for this site
- Footer
  - Added copyright, link to your medium page, and link to my LLC, hope that's ok

# References

- Current site
  - http://denverfreelancing.com/
  - github: https://github.com/dhornbein/denverfreelancing.com/
- MDB
  - https://mdbootstrap.com/
- URL for group photos
  - https://drive.google.com/drive/folders/1c907O0EON8ZX5ywbNuK1jvKsT5MB_KW4
- Coding standards site: http://codeguide.co/
  - MDB recommends following it, and I did when I needed to make a choice
  - For example, added "IE compatibility mode" to each page:
    - `<meta http-equiv="X-UA-Compatible" content="IE=Edge">`


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



