# jiffie

## What is it?

_jiffie_ is a docker based solution which aims to quickly create a php application skeleton with quality control at the root of the project.

## Why is it?

So I could bootstrap my work quickly.

## Why not create a composer create project thingy?

I wanted to use docker and not require the OS to have php or composer and found it clunky to try and make a composer project in a docker container.

## Okay how does it work?

```bash
git clone --depth=1 --branch=master git@github.com:Tom-Millard/jiffie.git [your new project name]
cd [your new project name]
rm -rf .git
docker compose build
docker compose run php bash setup
rm setup
```

## Why does it have a stupid name

_you have a stupid name_

## todo

- Get travis to build this and test it
- Create some common CI examples
