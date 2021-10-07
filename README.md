Handbook inspired by GitLab handbook first approach to document the things that I have found to be useful/important in setting up engineering teams in a startup environment.

# Installation

The following are basic steps to get Jekyll running on a local development environment and configured with GitHub Pages.



## Installing Jekyll

If you have already install the following:

1. Ruby
2. Bundler, a Ruby **gem** to manage you project's dependencies
3. Jekyll

## Set Up your site

Create a new empty repository on GitHub for your Project say `my-project`.

> **Warning:** Remove any visible files, such as the README.MD to another directory
> copy the files back once the site has been set up.

Run the following command to create all the necessary starter files and directories:

    > jekyll new .

> **TODO:**
> Add stuff in here about the Gem and config.yml files, in particular the use of the _config_lcoal.yml file for the just-the-docs

The [`just-the-docs`](https://pmarsceill.github.io/just-the-docs/) theme has been used for layout. This theme separate local and remote theme definitions:

    > theme: "just-the-docs"
    > remote_theme: pmarsceill/just-the-docs

To manage this separate configuration files have been defined for running the site locally versus in GitHub Pages.

Run the following commands to update the Gemfile.lock and build the project

    > bundle update

    > bundle install

Startup the local Jekyll server, not the specification of the local configuration file:

    > bundle exec jekyll server --config _config_local.yml --watch

# Useful references:

- [Getting starteg with Jekyll and GitHub](https://www.aleksandrhovhannisyan.com/blog/getting-started-with-jekyll-and-github-pages/)
