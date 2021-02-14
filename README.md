# planet-bitfolk
Configuration for [Planet BitFolk](https://planet.bitfolk.com/) and associated
projects.

## Purpose
[Planet BitFolk](https://planet.bitfolk.com/) is a feed aggregator. It
publishes feeds of articles and updates by [BitFolk](https://bitfolk.com/), its
customers and hangers-on.

## Adding your feed

### Whose feeds are welcome
Generally, if you are a customer or someone active in and around BitFolk then
you may add your feed. If you cease to be active then we'd like you to remove
it again, or we might do that for you, if we notice that we haven't seen you
around in a long time.

### How to add your feed
In decreasing order of preference:
* Edit the
  [config.ini](https://github.com/bitfolk/planet-bitfolk/blob/main/config.ini)
  here in this repository and submit a pull request.
* Or open an issue asking to be added.
* Or find some way to contact [grifferz](https://github.com/grifferz) and ask
  him to add you.

We prefer feeds that give the full content of your articles (not just a
synopsis / first paragraph), but if you really don't want to show the full
article then that's okay. Discoverability is the main thing.

Please add your feed in alphabetical order (by the `name` parameter).

## Content guide
Content doesn't have to be about BitFolk or technical in nature.

Please consider a diverse readership and try not to be annoying. If you are
excessively annoying (in the sole determination of BitFolk) then you may be
asked to provide a tagged feed without such posts, or else have your feed
removed.

Your feed should be in English.

Advertising content (as distinct from just posts about what you're working on
etc.) is not welcome.

Please only add *your own* feeds, not those of anyone else.

## Operational notes
### It's dead, Jim
The static site is currently generated by [the planet-venus
aggregator](https://github.com/rubys/venus). This appears to be
upstream-abandoned Python 2-only code that has [recently been removed from
Debian](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=940982) for that
reason.

That means that running it after the end of the Debian buster release may
become problematic. Venus seems to still be in use by many many aggregator
sites. The alternatives don't look great so for now we'll cross that bridge
when we come to it.

### Theme
The theme in use is the stock Venus "asf" theme, slightly modified.

If after installing Venus you clone this repository and run:

```
$ planet ./config.ini
```

then it should generate a copy of the site for you.
