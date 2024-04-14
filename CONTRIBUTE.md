

## Code Management
The project is based on [GitHub Pages](https://docs.github.com/en/pages) and [Jekyll](https://jekyllrb.com). Explore their websites for more information and troubleshooting. 

### Quick Start
1. Install prerequisites
```
sudo apt-get install ruby-full build-essential zlib1g-dev
gem install jekyll bundler
```

2. Run it locally:
```
bundle exec jekyll serve
```
3. Browse [http://localhost:4000](http://localhost:4000/)

### Development
The project is powered by [Bootstrap](https://getbootstrap.com/) and uses [Jekyll Layouts](https://jekyllrb.com/docs/layouts/) to organize the content. The main layouts are:
- **Default** as the base html for all other layouts
- **Home** for the homepage.
- **Post** for a single post page.
- **Simple** for all remaining page without much complexity (like `about us` page)

Review the [issues page](https://github.com/NaarvanMag/naarvanmag.github.io/issues) to start contributing ;)


## Content Management
Most of the contents are organized in mardown pages with a simple configuration.
#### Add a new category
 Categories are set up as folders in the project. To create a new category:
 1. Add a new folder in the root folder and name it as the name of the new category. It appears in the main page as a new section.
 2. Add a new custom html page to `pages/archive` folder and add its link to the header in `_layout/default.html`.
 3. Put the related documents (like cover page and pdf file) to `assets/archive` folder.

#### Add a new post
Posts are set up as markdown pages in each category folder. To create a new post:
1. Add a new markdown page using the existing template and add the post content in the markdown format. It's adviced to use the same template, as all posts are using the same layout.
2. Put the post tile to `assets/tile` folder (it should be a square image) and fill the required configurations in the markdown file.
3. The post appears in the main page.

#### Add a new page 
Page are supported as both html and markdown files. Html files might be fully customized, markdown files uses a predefined layout.
1. Add a new page (custom html  or markdown file) to `pages` folder.
2. Add its link to the header or footer in `_layout/default.html` to make it accessible.