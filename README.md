phIndex
=======

Simply copy one of the `index.php` files into the directory you want to index. Change excludes and formatting as needed.
The script will take care of replicating itself in the sub-directory tree.<br>

The visual style of the index generated by `index-simple.php` apes nginx behaviour. The other one `index-fancy.php` outputs
a visually more appealing index. - Feel free to change the Stylesheets, though ;)

If you ever want to update the script, simply update the one that's at the root of your index hierarchy. The script will
compare timestamps of index.php files in sub-directories and replace them if needed.


## Why?!
While nginx is the web server of my choice its HttpAutoindexModule neither
supports an option to exclude files nor does it sort numerical names correctly.<br>
`10` would be placed after `1` but before `2` - this script resolves this issue.
