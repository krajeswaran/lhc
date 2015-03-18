lhc
===

*NOTE*: This was done before Jekyll powered static sites became cool. 

A simple rolodex-style static site content generator for a internal tools website. Uses Ruby, Roundabout.js and Bonsai gem.


How to add a new tools section
------------------------------
1. Clone this repo
2. Navigate to `content/index/` folder
3. Copy a sample folder, say `1.linuxgoodness` and rename it to something meaningful. The prefix determines the order your tools section will be rendered
4. Modify the `default.yml` file. The format is easy to figure out, just beware, YAML is space sensitive..
5. Add a logo, with any filename under `logo` folder
6. Run `bonsai --repot` in lhc. This will re-generate the site under `output/` directory. Alternatively, you can use `bonsai -c` for hacking, until you are ready to move the site to root.
7. Copy your output directory to `/var/www/`. You need sudo for this.
```
cd output
sudo cp -R . /var/www/
```
8. That's it. Refresh!
9. Make sure you commit your changes back to this repo

