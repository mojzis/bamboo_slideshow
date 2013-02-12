#Bamboo Slideshow Documentation

##Required third party modules and libraries:

* [entity](http://drupal.org/project/entity)
* [entityreference](http://drupal.org/project/entityreference)
* [features](http://drupal.org/project/features)
* [flexslider](http://drupal.org/project/flexslider)
* [libraries](http://drupal.org/project/libraries)
* [views](http://drupal.org/project/views)
* [views_slideshow](http://drupal.org/project/views_slideshow)

Install the third party modules above as usual. 
See [Installing contributed modules (Drupal 7)](http://drupal.org/documentation/install/modules-themes/modules-7) for more info. 

**Typical locations for Drupal modules:**

* */sites/mysite.com/modules*
* */sites/all/modules/contrib*
* */sites/all/modules*

-----

* Install the Bamboo Slideshow Feature (this module) as per above or if you have a "custom" directory under /modules
* Install the [flexslider library](http://flexslider.woothemes.com/) in */sites/all/libraries*

When you activate the Bamboo slideshow module, you will be prompted to activate the dependent modules. Be sure to agree to this option to activate these dependent modules. 

##Create Slideshow Content

Now that you have installed everything (and hopefully it went well), create some content. 

"Content > Add content > Bamboo Featured" (which is the name of the new content type this module creates after activation.) Or simply go to /node/add/bamboo-featured. 

### -- Node Fields
When you create slideshow content, there are a number of fields to be aware of. 

**Title** - standard Drupal title which ends up as the title of the slide. 

**Slide Text** - This is the text displayed in under the slide. The slideshow truncates this at 110 characters so ideally you should not enter any more than that. 

**Content Link Reference** - This option is if you would like to link your slide to another piece of existing content in your site. This option is ideal if retrofitting the slideshow to an existing site that has a lot of content.

##Place the slideshow block
The feature creates a few blocks. 


