# siamscsdsu.github.io

## About

This is the code behind the SDSU Computational Toxicology Website. It uses Github Pages and Jeykll as its functionality (for posts, etc). The website was originally developed in October 2023 by forking the following Jeykll Theme: [Mudana](https://github.com/wowthemesnet/mundana-theme-jekyll). Significant changes have been made from the theme by Ashley Schwartz ([https://ashleyschwartz.com/](https://ashleyschwartz.com/)).

## Website Description and Organization

- `_pages`: This folder contains the content for the pages on the webpage. The main pages are: `about.md`, `executive-board.md` and `contact.md` (the homepage is in the base directory: `index.html`)
    - `about.md`: The about page. Feel free to edit information in this file if you wish. Notice the header. This includes imporatant functionality information and should not be modified. The only modification would be the image if you wish to change the image on the sidebar. 
    - `people.md`: The people page. Most of this page content is just the images of the members. The information about the board is in `_config.yml` so upon member change, edits should be made there. Only note here is all board member images should be `.jpg` and located in `/assets/images/team/`.
    - `contact.md`: The contact page. Probably doesn't need to be modified but you definitely can!
- `_layouts`: This folder contains the html for the pages on the webpage. I do not recommend making any modifications to files in this folder. These are layouts, and the actual page content will be included on a `markdown` file in the `_pages` directory. 
- `_includes`: This folder contains snippets of html often included in layouts. I do not recommend making any modifications to files in this folder. If you have added a new page and want to include that in the menu, that would be in `menu-header.html`.

## Make Changes to the Website

You have some options on this, depending how comfortable you are with GitHub. The main website functionality is basically ready to go and most future modifications would only be in the `_config.yml` file and and additions to `_posts` folder to announce events (and images for these posts). You can do this directly in GitHub if you are logged into the SIAM SC SDSU GitHub Page. 

## Host the Website Locally

It is advantageous to host the website locally when making modifications to see any changes in real time. I recommend the following steps:

1. Make your personal github a collaborator on this repo.
    - This will allow you to push to this main branch but will not mess with you GitHub login on your computer.

```
cd /Users/ashleyschwartz/Documents/Research/sdsucomptox/sdsucomptox.github.io
bundle exec jekyll serve
```