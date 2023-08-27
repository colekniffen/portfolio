# Portfolio

A basic portfolio to showcase my work! Check it out <a href="https://colekniffen.github.io/portfolio/">here</a>!

#### Table of Contents:

<a href="https://github.com/colekniffen/portfolio#how-to-customize-this-template">How to customize this template</a></br>
&nbsp;&nbsp;&nbsp;<a href="https://github.com/colekniffen/portfolio#creating-a-new-project-page-and-adding-it-to-the-homepage">Creating a new project page</a></br>
&nbsp;&nbsp;&nbsp;<a href="https://github.com/colekniffen/portfolio#adding-images-to-the-project-gallery">Adding gallery images</a></br>
<a href="https://github.com/colekniffen/portfolio#publishing-with-github-pages">Publishing with Github Pages</a></br>
<br />
<br />

## How to customize this template

- Image assets to add for projects, header photo, or the favicon should go in the `assets/images` folder
- For every new project page, make a copy of `project-template.html` and keep it in the `project-pages` folder
- All styling is located in the `css` folder if I feel like changing up the styling.
- The `js` folder holds a simple script file to add any custom Javascript into.
  <br />

### Creating a new project page and adding it to the homepage

1. Make a copy of `project-template.html` in the `project-pages` folder and rename it to `<project-name>.html`
2. Open `index.html` and find the `div` with `className='project-container'`
3. Add a new project card into that div. Here's the template for a project card:

```
  <div class="project-card">
    <img src="./assets/images/IMAGE_NAME" class="project-image">
    <div class="project-card-text-container">
      <div class="subheader-text project-title">PROJECT_NAME</div>
      <div class="body-text project-card-text">SMALL_PROJECT_DESCRIPTION</div>
    </div>
    <a class="button" href="./project-pages/PROJECT_PAGE_NAME.html">
      <span class="button-text">Read More</span>
      <image src="./assets/icons/arrow-right.svg" class="right-arrow-icon"/>
    </a>
  </div>
```

4. Change `PROJECT_PAGE_NAME.html` to the name of the new html file you copied from the project template
5. The project page is now linked to the homepage! Customize the page and `"project-card"` to your heart's content.
   <br />

### Adding images to the project gallery

1. Make sure the images that I want to show are added to the `assets/images` folder
2. Open the project page I want to edit and find the `div` with `class="project-gallery-content"`
3. To add an image, copy one of the two templates below and paste them into the `project-gallery-content`

```
Full Width Image:

    <div class="gallery-image-container">
      <img src="../assets/images/IMAGE_NAME" class="gallery-image">
      <span class="image-caption">IMAGE_CAPTION</span>
    </div>


Half Width Image:

    <div class="gallery-image-container half-width">
      <img src="../assets/images/IMAGE_NAME" class="gallery-image">
      <span class="image-caption">IMAGE_CAPTION</span>
    </div>
```

4. Change IMAGE_NAME to the filename of the image I added to `assets/images` and IMAGE_CAPTION to whatever caption I want (or remove it, I don't mind)
5. Refresh the project page in the browser and boom! The image has been added to the gallery.
   <br />
   <br />

## Publishing with Github Pages

Github Pages allows us to host this website for free! It's pretty simple to set up as well.

1. Head to `Settings` on the repository
2. The repository will need to be public for this work (if it's not, navigate to `General` and scroll all the way down to `Change repository visibility`. Make it public)
3. Navigate to `Pages` in the sidebar
4. For `Source` choose `main` from the dropdown. Save the changes.
5. That's it! Github should give you a URL that your website is published on (give it a few minutes to update).
6. To add a custom domain (i.e. yourname.com), follow this guide: https://medium.com/codex/add-a-custom-domain-to-your-github-pages-personal-website-53ab40e7c7d0
   <br />
   <br />
