# Screenshot URLs script

A node script to take screenshots of webpages using puppeteer.

## Installation

Run `npm install` or `yarn install`

## Generating screenshots

```
node index.js [--url <url>] [--input <path>] [-dest <path>] [--width <pixels>] [--height <pixels>] [--format <format>] [--wait <milliseconds>]
```

### Single

To generate a single screenshot, the only required argument is URL. The output filename can be automatically generated.

e.g.

```
node index.js --url="https://www.google.com/" --width=1600 --height=900
```

will generate a screenshot with the dimensions 1600 by 900 pixels inside the `./output` folder. The auto-generated filename contains of a timestamp and sluggified version of the URL.

### Bulk

Make a text file with each URL separated by a new line.

e.g.
```
https://www.google.com
https://www.bing.com
```

then give the command the path to the input file:

```
node index.js --input=pages.txt
```
