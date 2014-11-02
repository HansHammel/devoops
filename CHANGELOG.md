## Bug Fixes
### 11/02/2014
- added two missing images (not_available-generic.png, waiting-generic.png)
- changed orphaned page_locked.html link to #
- changed orphaned html5shiv and respond.js links (on cdnjs)
- optimized all images like so:
    for /R %v in (*.jpg) do jpegtran -copy none -optimize -progressive -outfile "%v" "%v"
    for /R %v in (*.gif) do gifsicle -O1 -o "%v" "%v"
    for /R %v in (*.png) do pngout "%v" "%v" /y
- changed getScript to getScriptCached and added some code for cache support, now we get all a-grades on gtmetrix.com for speed optimization (on a cache enabled server!)
- added options for async and cached ajax
- reformatted code (sorry, bad habit!)
- optimized css (mostly redundant measurement units)
- fixed image links of amchart to correct location in plugin folder
- extended .gitignore file
- changed some documents (styling and names)
- added CHANGELOG.md
- maybe more...