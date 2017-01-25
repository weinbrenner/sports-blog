# Sourcecode for my blog sports.weinbrenner.name
A [Jekyll](https://jekyllrb.com/) based blog built upon the [Trophy](http://thomasvaeth.com/trophy/) theme.

### _config.yml

#### Site Settings
    email: 
    baseurl: ""
    paginate: 5
    paginate_path: "/blog/page-:num"
    google_analytics: UA—XXXXXXXX-X

* ````email```` - Your email for the contact card and the footer
* ````baseurl```` - Path of blog if adding this on to another website
* ````paginate```` - Number of blog posts per page
* ````paginate_path```` - URL structure of paginated pages
* ````google_analytics```` - Option field to replace with correct Google Analytics code

#### SEO Settings
    title: 
    description: 
    url: ""
    twitter_username: 
    default_img: 

* ````title```` - Title of blog
* ````description```` - Description of blog (recommended to not go over 160 characters)
* ````url```` - URL of main website
* ````twitter_username```` - Twitter username
* ````default_img```` - Image that will appear when posting links on social networks

#### Profile Settings
    name: 
    profile_img: 
    profile: 
    social:
      github: 

* ````name```` - Full name for SEO purposes
* ````profile_img```` - Image for the profile card (size to 2000x1200px)
* ````profile```` - Short description that will be in the profile card
* ````social```` - List of social networks for icons in the contact card and the footer ([Font Awesome](http://fontawesome.io/) is used, so only match the name of the icon, but do not include ````fa-````)


#### Build Settings
    include: ["_categories"]
    exclude: []
    permalink: /:year/:month/:day/:title/

* ````include```` - Folders that are not automatically included in Jekyll
* ````exclude```` - Folders that are excluded from `_site_`
* ````permalink```` - URL structure of blog posts

### _posts
    ---
    layout: post
    title: ""
    date: 
    categories:
    description: 
    image: 
    image-sm:
    ---

This is the YAML front matter block for blog posts.
* ````layout```` - This field will always be post
* ````title```` - The title of the blog post
* ````date```` - The date that will appear on the blog post
* ````categories```` - Optional field that can be entered as an array or a list
* ````description```` - Optional field for SEO (recommended to not go over 160 characters)
* ````image```` - The blog theme was designed for 2000x1200px images (optimize your images because this is a picture heavy theme)
* ````image-sm```` - Optional field for card layouts for image optimization and page speed (designed for 500x300px images)

### _categories
    ---
    layout: default
    title: New Category
    description:
    permalink: /category/new-category/
    ---
    {% include category.html %}

* ````layout```` - This field will always be default
* ````title```` - Name of the category
* ````description```` - Optional field for SEO (recommended to not go over 160 characters)
* ````permalink```` - URL for the category

## Licenses
This source code is licensed under the MIT License.
The blog content is licensed under the [Creative Commons License]()https://creativecommons.org/licenses/by/4.0/)
