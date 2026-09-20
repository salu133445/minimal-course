# Minimal Course

Minimal Course is a Jekyll template for course websites. It is designed to be **as minimal as possible** yet easily maintainable for the instructor. The template is adapted from [minimal](https://github.com/orderedlist/minimal) by [orderedlist](https://github.com/orderedlist).

**Live demo**: [hermandong.com/minimal-course](https://hermandong.com/minimal-course/)

## Example Course Websites

Example course websites built with this template include:

- [Music and AI](https://hermandong.com/teaching/pat463_563_fall2026/) (PAT 463/563, University of Michigan)
- [Generative AI for Music and Audio Creation](https://hermandong.com/teaching/pat464_564_winter2026) (PAT 464/564, University of Michigan)
- [Creative Coding](https://hermandong.com/teaching/pat204_504_fall2026) (PAT 204/504, University of Michigan)

## Features

- Light/dark mode switch
- Audio and video players supports
- Math supports with MathJax
- Icon supports with Font Awesome
- Handy formatting shorthands for highlights, colors, fonts, etc.

Features demo: [hermandong.com/minimal-course/features](https://hermandong.com/minimal-course/features)

## Repository Structure

```text
┬─ _data
│    └─ icons.yml                Icons configurations (Fontawesome icons)
├─ _includes
│    ├─ audio.html               Helper function for audio players
│    ├─ link.html                Helper function for icon links
│    ├─ mathjax.html             HTML header for MathJax supports
│    ├─ video.html               Helper function for video players
│    └─ youtube.html             Helper function for YouTube players
├─ _layouts
│    └─ default.html             Default HTML skeleton
├─ _sass
│    ├─ fonts.scss               Stylesheet file for fonts
│    ├─ highlight.scss           Stylesheet file for code highlighting
│    └─ minimal-course.scss      Stylesheet file
├─ assets
│    ├─ css                      Stylesheet files
│    ├─ fonts                    Font files
│    ├─ js                       Javascript files
│    └─ webfonts                 Webfont files
├─ hw1                       *
│    ├─ example_image.jpg    *   An example image file
│    ├─ index.md             *   Main file for the HW 1 page
│    ├─ example_audio.mp3    *   An example audio file
│    └─ example_video.mp4    *   An example video file
├─ slides                    *
│    └─ example_slide.pdf    *   An example slide file
├─ .gitignore                    Git configuration file
├─ Gemfile                       Ruby dependencies file (for local development)
├─ favicon.ico               *   Website shortcut icon
├─ features.md               *   An example subpage showing the features
├─ index.md                  *   Homepage of the course website
├─ project.md                *   An example subpage showing project instructions
├─ README.md                     This file
├─ _config.yml               *   Jekyll configuration file
└─ environment.yml               Conda environment file (for local development)
```

You should update the files marked with a `*`.

## Usage

1. Create a new repository based on Minimal Course ([Click here](https://github.com/salu133445/minimal-course/generate))
2. Navigate to "Settings > Pages" in the GitHub repository you just created
3. Under "Branch", change "None" to "main" and click "Save"
4. Refresh after a short while, you should see a link showing up at the top of the page in the form of `https://USERNAME.github.io/REPONAME`
5. Your course website is now live! Click the link to take a look!

Now, you may start editing your course website:

1. Update `_config.yml` with your course information
2. Edit the `index.md` file to update the homepage of your course website
3. Add markdown (`.md`) files to create subpages (Alternatively, create a folder with an `index.md` file inside it)
4. Replace `favicon.ico` to something you like

## (Advanced) Setting Up a Local Development Environment

Follow the following steps to create a Conda environment to serve the website locally:

1. Create a Conda environment: `conda env create -f environment.yml`
2. Activate the Conda environment: `conda activate minimal-course`
3. Install Jekyll: `gem install jekyll`
4. install Ruby dependencies: `bundle install`
5. Test the Jekyll installation: `bundle exec jekyll -v`

Once you have the environment set up, you may serve the website with the following commands:

1. Activate the Conda environment: `conda activate minimal-course`
2. Serve the website: `bundle exec jekyll serve`

## Sponsoring

If you enjoy Minimal Course, I would be very happy if you buy me a bubble tea 🧋 through [GitHub Sponsors](https://github.com/sponsors/salu133445)! 😁
