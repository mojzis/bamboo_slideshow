#Drupal Bamboo Slideshow Documentation

Bamboo Slideshow is a Feature (module) for [Drupal 7](http://drupal.org/project/drupal). It uses Views, Views Slideshow and Flexslider so it's responsive out of the box. You can [see a demo of it here](http://bamboo.themehuis.com/bamboo-featured-content-slideshow). Bamboo Slideshow is a companion module for the [Bamboo theme](http://drupal.org/project/bamboo) on drupal.org by [Danny Englander](http://highrockmedia.com/) ([@highrockmedia](https://twitter.com/highrockmedia)) The Feature works well with the Bamboo theme but should also work well with other Drupal 7 themes. 

-----

##Required third party modules and libraries:
* [Entity API](http://drupal.org/project/entity) - 7.x-1.0
* [Entity Reference](http://drupal.org/project/entityreference) - 7.x-1.0
* [Features](http://drupal.org/project/features) - 7.x-2.0-beta1
* [Flexslider (module)](http://drupal.org/project/flexslider) - 7.x-2.x-dev (2013-Jan-25 or newer)
* [Libraries api](http://drupal.org/project/libraries) - 7.x-2.0
* [Views](http://drupal.org/project/views) - 7.x-3.5
* [Views Slideshow](http://drupal.org/project/views_slideshow) - 7.x-3.x-dev (2012-Apr-24 or newer)
* [Chaos tool suite (ctools)](http://drupal.org/project/ctools) - 7.x-1.2

Install the third party modules above as usual.
See [Installing contributed modules (Drupal 7)](http://drupal.org/documentation/install/modules-themes/modules-7) for more info. 

**Typical locations for Drupal modules:**

* */sites/mysite.com/modules*
* */sites/all/modules/contrib*
* */sites/all/modules*

-----

* Install the Bamboo Slideshow Feature (this module) as per above or if you have a "custom" directory under /modules
* Install the [flexslider library](http://flexslider.woothemes.com/) in */sites/all/libraries*  

Note that when you download flexslider, it will look like "woothemes-FlexSlider-06b12f8" or similar. You should rename this folder to "flexslider", all lower case so your final end result is */sites/all/libraries/flexslider*.

When you activate the Bamboo slideshow module, you will be prompted to activate the dependent modules. Be sure to agree to this option to activate these dependent modules. 

##Create Slideshow Content

Now that you have installed everything (and hopefully it went well), create some content. 

"Content > Add content > Bamboo Featured" (which is the name of the new content type this module creates after activation.) Or simply go to /node/add/bamboo-featured. 

### -- Node Fields
When you create slideshow content, there are a number of fields to be aware of. 

**Title** - standard Drupal title which ends up as the title of the slide. 

**Slide Text** - This is the text displayed in under the slide. The slideshow truncates this at 110 characters so ideally you should not enter any more than that. 

**Content Link Reference** - This field option is if you would like to link your slide to another piece of existing content in your site. This option is ideal if retrofitting the slideshow to an existing site that has a lot of content. For this option, use the **View: Featured Slideshow: Content Reference Slideshow Block** on the blocks admin page. 

**Page content** -- This field option is if you would like to have your slideshow linked to the origin node itself. For this option, use the **View: Featured Slideshow: Link-to-self Slideshow Block** on the blocks admin page. 


##Choose and Place a Slideshow Block
The Feature creates two blocks as mentioned above. You can see these on the blocks admin page or at */admin/structure/block*

1. **View: Featured Slideshow: Link-to-self Slideshow Block**
2. **View: Featured Slideshow: Content Reference Slideshow Block**

Use the first block if you are using the **Page Content field**, use the second block if you are using the **Content Link Reference** option. See "Node Fields" above for more info. Ideally you want to place this in a block region that is a full width of your theme. In the Bamboo theme, the region is called "Hero 1"


##Support
This Feature is free and licensed under GPL. However, if you require support, I can offer this on a paid basis either hourly or per project. Please do not open an issue for this in the Bamboo issue queue on drupal.org, [contact me directly](http://highrockmedia.com/contact-us). 



