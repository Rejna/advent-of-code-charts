# Advent of Code Charts

This is a [fork](https://github.com/jeroenheijmans/advent-of-code-charts) of [unofficial](#license-and-affiliation-disclaimer) small hacked-up set of charts for a private leaderboard for [Advent of Code](https://adventofcode.com/). Its original author is Jeroen Heijmans. It has some small additional features and changes, done by me, and in this state isn't available in Chrome/Firefox extension stores.

## Disclaimers

It is *not* a well-architectured, well-written, neat, nice, fluffy, industry-strength piece of code.
Instead it's something fun I wanted to make, stepping out of my *normal* way of coding. NO WARRANTY!

## Developing

Install dependencies:

```sh
npm ci # or npm install
```

Serve a test website with the dummy data:

```sh
npm run start # runs 'serve' and 'watch' in parallel
```

And open up `http://localhost:3000`.

## Building

Run `build.ps1` or `build.sh` to re-create a `/build` folder which is a ready-to-go browser extension.
Test the extension by loading it in the browser.
For full reference, see Chrome's or Firefox's full documentation, but the basics are:

- Firefox: go to `about:debugging` and load a temporary addon (pick the `/build/manifest.json` file)
- Chrome: go to `chrome://extensions` and load unpacked extension (pick the `/build` folder)

Test by browsing to a private leaderboard and you should see charts popping up at the bottom.

## License and Affiliation Disclaimer

The code in this project is MIT licensed, with the explicit exception of `dummyData.js`.
That file contains JSON in a format thought up by the owner and creator of Advent of Code, but we suppose that using a small snippet of it like this falls under "fair use" (given for one that the AoC website itself suggests using the "JSON API" for integrations, albeit without spamming that API).

Note that "Advent of Code" and "AoC" are Eric Wastl's.
This project is not "official", and in no way (directly or indirectly) endorsed by- or affiliated to Advent of Code and its creator/owner.
Read more [about Advent of Code](https://adventofcode.com/2021/about) to learn about the project itself.

**Oh, and of course, please [consider donating to _Advent of Code_ itself](https://adventofcode.com/2021/support)!**

## Example

Here's what it should more or less look like:

![example-001.png](example-001.png)
