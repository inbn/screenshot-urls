# Screenshot URLs script

A node script to take screenshots of webpages using puppeteer.

## Installation

Run `npm install` or `yarn install`

## Generating screenshots

The only required argument is URL. The output filename can be automatically generated.

```
node index.js [--url <url>] [-dest <path>] [--width <pixels>] [--height <pixels>] [--format <format>] [--wait <milliseconds>]
```

e.g.

```
node index.js --url="https://www.google.com/" --width=1600 --height=900
```

will generate a screenshot with the dimensions 1600 by 900 pixels and output it here: /.output/20190316T171616_httpswww.google.com.jpg
