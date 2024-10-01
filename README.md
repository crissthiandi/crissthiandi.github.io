The repo for my website.

### About the Technology that I used

This personal website uses many technologies to work, from bash code (.sh) to R language (for Statistical Computing).
The next list tries to list all technologies and get info about them.

* [R][R]
    1. [RMarkdown][RM] to generate .md via [pandoc](https://pandoc.org/).
    2. [TidyVerse][TV] (Statistical Framework)
* [Ruby][Ruby]
    1. [Jekyll (framework)][jekyll]
    2. [Chirpy (theme)][chirpy]
    3. [Bundle gem][bundle] (Generate a project skeleton)
* Shell (to make a [CD][CD])
* [Github Actions][ga] (to build files previous to deploy)
* Js, HTML & CSS (Classic)
* [Linux SO](https://ubuntu.com/download)


[bundle]: https://bundler.io/man/bundle-gem.1.html
[CD]: https://en.wikipedia.org/wiki/Continuous_deployment
[chirpy]: https://github.com/cotes2020/jekyll-theme-chirpy/
[jekyll]: https://jekyllrb.com/
[R]: https://www.r-project.org/
[Ruby]: https://www.ruby-lang.org/en/
[ga]: https://docs.github.com/en/actions
[RM]: https://rmarkdown.rstudio.com/
[TV]: https://www.tidyverse.org/

## Install in wsl or linux OS

Run dependencies installer

```bash
sudo apt-get install ruby-full build-essential zlib1g-dev
```

Check has installed ruby 2.5.0 or higher, ruby gem, gcc, g++, make, and bundler

```bash
ruby -v
gem -v
gcc -v
g++ -v
make -v
bundler -v
jekyll -v
```

If any of dependencies is not installed, install using google, for example for bundler if i use ruby 2.7.0 the command is:

```bash
gem install bundler -v 2.4.22
```

Is easy to install any dependency, just need to be patient, do research and read the error messages. Sometimes the error messages are very clear and tell you what to do. Especially when you are using a ruby version minor that 3.0.0.

## Run the project

first you need to run installer dependencies and then run the project

```bash
bundle install
bundle exec jekyll serve
```