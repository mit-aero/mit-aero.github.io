# AeroWiki

## Usage

- Open the website [AeroWiki](https://mit-aero.github.io/wiki)
- Search for the article
- Read whatever you want.

## Contributing

- ### Clone the repository
    - Run `git clone https://github.com/mit-aero/mit-aero.github.io`
- ### Add your markdown pages to `/wiki` directory
    - Learn how to write markdown.
    - Edit markdown pages in any editor (Recommended editors are VSCode with [markdown-editor](https://marketplace.visualstudio.com/items?itemName=zaaack.markdown-editor) extension or [ghostwriter](https://ghostwriter.kde.org/))
    - Add appropriate tags to help in search.
    - Add your pages to `/wiki` directory.
- # Push changes
    - Commit and push your changes with
    ```
    git add .
    git commit -m "[Your commit message]"
    git push
    ```
   
---
Below is the original README of the Jekyll template. Read if you want to edit the layout or style of the website.

---

# Personal Wiki / Digital Garden and Static Blog Site Setup

This is a template for a personal site, made with GitHub pages. 

![](resources/pw_screen1.png)

It uses jekyll, and comes with all the features you need to set up your digital garden / personal wiki (and a minimalistic blog). Available features include:

- Search (with a tagging system)
- Responsive design
- Fast loading times
- Markdown notes (easy to import or export from other tools)

Start using a note-taking system without having to invent one from scratch! Easily share your notes with other people by linking them to this site (which can be hosted for free on GitHub pages or netlify).

Original blog post: [How to Set Up Your Own Personal Wiki](https://strikingloo.github.io/personal-wiki-set-up). Additional reading: [Reflections on Note-Taking and Digital Gardening](https://strikingloo.github.io/reflections-digital-gardening).

## Forking this repo

If you want to build your own personal wiki / personal site using this template, all you have to do is:

- Fork this repo.
- Set up the values in `_config.yml` for your twitter username and Google Analytics ID.
- In the folder `wiki` you can put your own markdown notes, setting them with a title, tags and description. Use the example template as reference.
- Markdowns in the `_posts` folder it follow the same format, but their names must start with a date in format YYYY-MM-DD.
- Go to `_layouts` to see the HTML templates for each page kind. You can fiddle around with them.
- Customize `wiki/index.html`, the `index.html` on base directory (homepage) and `about/index.md`, as they are supposed to contain a personal description. Also update the social networking links on `_layouts/default.html`'s footer so they point to your networks. These include support for fontawesome icons. In that footer is also a path to the default twitter image, though each article or post can have its own image (specified in header).
- To change up the style, just edit `css/main.css` and run `minify_css.sh` to minify (or change the default layout to import the unminified css instead). You can find many good CSS templates that are free in this [Free Jekyll Themes Gallery](https://jekyllthemes.io/free).

To run the site locally, run

```
sudo gem install rails
sudo gem install jekyll
sudo gem install jekyll bundler
cd ~/this_project

bundle init
bundle install
bundle add jekyll
bundle exec jekyll serve
```
