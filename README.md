#Using the site

---
* Install hugo in your system. Check below for steps.
* Copy git folder and place it in `HUGO` directory.
* Run `cd hugo_sample`
* Start the hugo server. Steps given below.





#Getting started with Hugo Framework

---
Checkout https://gohugo.io/getting-started/quick-start/ for getting started.
##Installing in windows
* Goto https://github.com/gohugoio/hugo/releases.
* Find the release for windows in the bottom of the page and download the zip file.
* Create a new directory `Hugo/bin` and extract the files in zip folder in to the new directory.
* Add to `PATH` the new path created for `bin`.
* Run `hugo version` in command prompt to see whether hugo is installed.

##Installing in other OS
* Check https://gohugo.io/getting-started/installing/
##Creating a new site
* Run `hugo new site site-name` in the command prompt and a new folder named site-name will be created.

##Adding  a theme
* First, download the theme from GitHub and add it to your site’s themes directory:
* Sample code\
`cd site-name`\
`git init`\
`git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke`
* Then, add the theme to the site configuration: In `config.toml` add `theme = "ananke"`.

##Adding some content
* Run `hugo new posts/my-first-post.md`.
* This will create `content/posts/my-first-post.md`.
* Change `draft: true` to `draft: false`.
##Start the Hugo server
* Run `hugo server -D`.
* Navigate to your new site at http://localhost:1313/

##Getting example site from the theme
* Copy the content of `themes/ananke/exampleSite` to `site-name`.
* Ensure that `theme` in `config.toml` matches the file name in `themes` directory.
* Start the hugo server and navigate to site.
* Customize files in `content/` to edit the example site.

##Creating a new theme
Refer https://retrolog.io/blog/creating-a-hugo-theme-from-scratch/ \
OR
https://levelup.gitconnected.com/a-quick-tutorial-on-hugo-templates-creating-your-theme-a4102b42a85f

##Variables
* Variables can only be used inside templates and layouts, not inside content.
* The basic syntax of go html template looks like this `{{ args }}`
* Example of variable:\
  `{{ .Title }}` is used for accessing the title for this page.
* Custom variables $ : Hugo also lets you create your own custom variables. Here you can store values to use in your layouts. To create a custom variable use the following notation:\
`{{ $myVar := value }}` : assigns value to $myVar\
`{{ $myVar }}` : prints $myVar
  
##Notes
* All the templates are placed inside the layout.



