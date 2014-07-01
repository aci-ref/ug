
### Setup

+ Follow the instructions for setting up `ruby` and `jekyll` using the Bundler method from
here: https://help.github.com/articles/using-jekyll-with-pages

+ Checkout the User Guide source code, using the `gh-pages` branch:

    ```bash
    git clone -b gh-pages git@github.com:aci-ref/ug.git
    ```  

+ Run `make` to build the website.  Point your browser to [http://localhost:4000](http://localhost:4000) to preview any changes you've made


### Create a new book chapter


1.  Create a new directory in the top-level of the project.  This will be the chapter's identifier, it should be consist of lowercase letters and hyphens.
    ```bash
    mkdir my-chapter
    ```

2. Create the chapter's index file, `my-chapter/index.markdown`.  Within the page's frontmatter, three variables need to be defined: 
    1. `layout`: Always set this to `chapter`.
    2. `authors`:  List all the authors who contributed to this chapter.  Their names will appear at the bottom of the chapter.
    3. `sections`:  List, in order, the sections of the chapter.  The content of each section is an separate markdown file located in the `_includes` directory.  The `name` attribute is the base name of the section's markdown file, and is also used as the named anchor in the generated HTML code.

1. The body of `my-chapter/index.markdown` only needs to include the `chapter-down` file:
    ```
    {% include chapter-body.markdown %}
    ```

1. See the sample [supercompter](supercomputer) chapter for examples of including images, code blocks, math formulas in LaTeX
