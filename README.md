A Github Pages website for David Watkins-Valls. Ph.D. Student and researcher at the [Columbia Robotics Lab](crlab.cs.columbia.edu). This template was forked from [academicpages.github.io](https://github.com/academicpages/academicpages.github.io). 

## To run locally (not on GitHub Pages, to serve on your own computer)
1. Clone the repository and made updates as detailed above
1. Make sure you have ruby-dev, bundler, and nodejs installed: `sudo apt install ruby-dev ruby-bundler nodejs`
1. Run `bundle clean` to clean up the directory (no need to run `--force`)
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
1. Run `bundle exec jekyll serve` to generate the HTML and serve it from localhost:4000
