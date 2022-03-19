# My Academic Website

Thanks to [Dominik Moritz](https://www.domoritz.de/) (one of my PhD co-advisors), who I shamelessly scraped/forked this [template/repo](https://github.com/domoritz/domoritz.github.io) from!


## Write

```
bundle exec jekyll post "My New Post"
```

## Run

```
bundle exec jekyll serve --livereload
```

## Run with Docker

```
docker run \
  --volume="$PWD:/srv/jekyll" \
  -p 4000:4000 -p 35729:35729 \
  -it jekyll/jekyll \
  jekyll serve --livereload
```
