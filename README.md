# graimon.github.io

GitHub Pages deployment repository for **https://cv.rayware.ninja**

This repository contains the built static files for the CV website. The source code is maintained in the [online-cv](https://github.com/graimon/online-cv) repository.

## How to Update

1. Make changes in the `online-cv` repository
2. Build the site:
   ```bash
   cd ../online-cv
   bundle exec jekyll build
   ```
3. Copy built files here:
   ```bash
   cp -R _site/* ../graimon.github.io/
   ```
4. Commit and push:
   ```bash
   cd ../graimon.github.io
   git add .
   git commit -m "Update CV"
   git push origin master
   ```

## Important Files

- `CNAME` - Custom domain configuration (do not delete)
- `assets/cv-*.pdf` - PDF versions of the CV (preserved manually)

## Theme Credits

Based on the [Online CV Jekyll Theme](http://webjeda.com/online-cv/) by Xiaoying Riley at [3rd Wave Media](http://themes.3rdwavemedia.com/).
