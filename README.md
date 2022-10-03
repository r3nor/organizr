# organizr
Bash script that organizes a folder's files. 0 dependencies. No installations. Just a bash script.

## The problem

My "Downloads" folder tends to get very messy. I wanted to have it tidy and clean, so I made this script to run it in a cronjob.

## Usage

[![asciicast](https://asciinema.org/a/wBLIYJpcJLWOquyrjb34HF1Vo.svg)](https://asciinema.org/a/wBLIYJpcJLWOquyrjb34HF1Vo)

```
bash organizr <mode> <source> [destination]
```

The `organizr` script can run in multiple modes. Use the `organizr -h` or `organizr` without any arguments to see the "help" message. Each mode focuses on a group of file types.

You can also organize *everything* with the `all` mode.

---

#### Examples

> The following example is a typical usage example. Here, `organizr` would scan the `~/Downloads` folder. As it is set to `video` mode it will only focus on videos, so it would take all the folder videos and put them in a `~/Downloads/Videos` folder. Now all the videos from the "Downloads" folder are gathered together in a single folder:
```
bash organizr video ~/Downloads
```

> You can also specify a destination folder:
```
bash organizr photo ~/Downloads ~/Photos
```
