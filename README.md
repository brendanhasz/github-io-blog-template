# github.io Blog Template

A template repo for a github.io blog site.



## Features

- $\LaTeX$ math rendering via [MathJAX](https://www.mathjax.org/)
- RSS feed (at `http://your_github_username.github.io/atom.xml`)
- Auto dark mode :sunglasses:
- Comments via [Disqus](https://disqus.com/)
- Post tags (on the main page can filter posts by tag)



## Setup

1. Create a new repo from this repository template (at the top of this repo's main page, click the "Use this template" button to create your own copy of this repo).  If you'd like your site to be at `http://your_github_username.github.io`, then name the new repository `your_github_username.github.io`.  Otherwise you can name it `whatever_you_want` and it will be at `http://your_github_username.github.io/whatever_you_want`.

2. Go to the repository settings for the new repository, and scroll down to the "GitHub pages" section.  From the dropdown, select "main" (or whatever branch you want to build the site from).  Then click "Save".

3. To test out your setup, in a browser go to `http://your_github_username.github.io` (or, if you gave the repo a custom name, `http://your_github_username.github.io/repository_name`) and you should see the main page!  Now you can edit the repo so it has your own info:

4. Edit `_config.yml` to contain information about you and your new blog in the "Personal info", "Blog info", and "Social links" sections.

5. Add an image of yourself to the `/assets/img` folder, and in `_config.yml`, update the value of `logo` to be the filename of that image.

6. Replace `/assets/img/favicon.ico` with one you want (otherwise it will just be the default github octocat one, you can use a web utility like https://favicon.io/ to convert normal images to favicons)

7. Replace `/assets/img/company_icon.png` with the logo of your company/university.

8. Replace `/assets/img/blog_og_image.png` with image you'd like displayed when people share a link to your blog (e.g. on twitter, linkedin, etc)

9. Replace `/assets/files/resume.pdf` and `/assets/files/cv.pdf` with your resume/cv (or delete em).

10. Delete the example blog posts in `_posts` and replace with your first blog post(s)! (see below)



## Adding new blog posts

To add a new post, just add a markdown file to the `_posts` folder!

The header of each post defines some important information (the lines surrounded by `---` at the top):

* `title`: the title for the post
* `date`: the date of the post.  Note you can actually write and post posts ahead of time, and they won't be displayed until the `date` in the header
* `description`: a shortish description for the post.  This will be displayed on the post list on the main page.
* `img_url`: path to the image you want to show for this post on the main page
* `tags`: a list of tags you want for this post.  On the main page you can filter posts by tag.
* `github_url`: (optional) a url to a github repository with code (or whatever) relevant to this post (will show a link at the top of the post)
* `colab_url`: (optional) a url to a Google Colab notebook relevant to this post (will show a link at the top of the post)
* `kaggle_url`: (optional) a url to a Kaggle notebook relevant to this post (will show a link at the top of the post)

See the example posts in the `_posts` folder for example markdown content, including sections, links, lists, code blocks, equations, images, etc.

You can add images for your post(s) in `/assets/img`.  I usually have a folder in `/assets/img` for each blog post, just to keep things tidy.



## Settings

### Dark mode

By default, dark mode will be used for people viewing the page with their computer/browser preferences set to "Dark".  To force the light theme, in `_config.yml` set `color_mode` to `light`.  Or, to force the dark theme, in `_config.yml` set `color_mode` to `dark`.  

### Comments

To enable comments on your posts via [Disqus](https://disqus.com/), first you'll need to sign up for a Disqus account and register your new site.

Then, in `_config.yml`, set `comments` to `true`, and set `disqus_shortname` to [your site's Disqus shortname](https://help.disqus.com/en/articles/1717111-what-s-a-shortname).



## Customization

The base html which serves as the template for all pages on the site is in `/_layouts/default.html`.  Edit it as you want!

The CSS for the site is in `/assets/css/` folder.

Other than that, it's just a regular github pages site, so see [all their documentation](https://pages.github.com/) about customization.



## Permissions

You can feel free to copy/use any of this without restrictions (MIT license).

The [headshot.svg file is CC-BY-SA by East718](https://commons.wikimedia.org/wiki/File:718smiley.svg) (but you'll probably be replacing that with an image of yourself).