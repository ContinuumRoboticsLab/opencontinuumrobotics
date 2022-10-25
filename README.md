# Open Continuum Robotics Project Website
This website is based on the [Minimal Mistakes Jekyll theme](https://github.com/mmistakes/minimal-mistakes).

Install Jekyll on your machine. Run

    bundle exec jekyll serve --watch  --future  

# How to contribute to the blog
- posts are written in [Markdown](https://www.markdownguide.org/basic-syntax/) (see posts in _posts folder for examples)
- filename YYYY-MM-DD-short.md (publishing date)
- add a new file to the _drafts folder (structured by category)
- add this header to each post

        ---
        title: "TITLE"
        author: your author abbreviation
        toc: true/false
        category: 101/coolCR/hands-on/history/opinion/research
        excerpt: short excerpt
        header:
            teaser: /assets/images/posts/teaserImageFilename
        ---
        your post goes here

- images for posts are stored in assets/posts folder
- select a teaser image for the post (500x300)
- once post is ready for publication move to the _posts folder
- if this is your first post, make sure that you create your author profile in _data/authors.yml

# Questions?
Contact jessica.burgnerkahrs@utoronto.ca