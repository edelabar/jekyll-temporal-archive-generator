jekyll-temporal-archive-generator
==============================

Yearly and Monthly Archive Index Generator for Jekyll

This generator was built to migrate my website from Wordpress to Jekyll but maintain the existing permalink structure.  I'm incredibly anal when it comes to nice URLs, so I needed an index page for each segment of my permalinked URLs.

##Credits##

This Generator is based on code from the Jekyll category page generator (http://recursive-design.com/projects/jekyll-plugins/) by Dave Perrett (http://recursive-design.com/) and the Monthly archive plugin for Jekyll (https://github.com/shigeya/jekyll-monthly-archive-plugin) by Shigeya Suzuki (https://github.com/shigeya) I'm not much of a Ruby dev, so this would not have been possible without their working examples.

##Usage##

To use it, simply drop this script into the ```_plugins``` directory of your Jekyll site and drop the ```monthly_index.html``` and ```yearly_index.html``` files into the ```_layouts``` directory of your site.  Feel free to edit the layouts and/or front matter as you see fit.

When you compile your jekyll site, this plugin will loop through your posts, and use the layouts above to generate a page for each year and month with a list of links to the individual posts.

###Example###

For instance, if you have the following posts:
 
* 2013-01-01-test-post-1.markdown
* 2014-01-01-test-post-2.markdown
* 2014-02-01-test-post-3.markdown

This plugin will create the following index files:

* 2013/index.html
* 2013/01/index.html
* 2014/index.html
* 2014/01/index.html
* 2014/02/index.html


Copyright (c) 2014 Eric DeLabar, http://ericdelabar.com/<br/>
Licensed under the MIT license (http://www.opensource.org/licenses/mit-license.php)
