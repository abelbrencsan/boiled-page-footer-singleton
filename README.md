
# Boiled Page footer singleton

Footer SCSS singleton for Boiled Page frontend framework. It is intended to create a footer with a short description, navigations, copyright, links to legal documents and other pages.

## Install

Place `_footer.scss` file to `/assets/css/singletons` directory, and add its path to singleton block in `assets/css/app.scss` file.

## Usage

### Classes

Class name | Description | Example
---------- | ----------- | -------
`footer` | Applies footer. | `<footer class="footer"></footer>`
`footer-nav` | Applies navigation area inside footer that contains a short description and navigation groups. Tip: use grid component to align children elements. | `<div class="footer-nav"></div>`
`footer-nav-group-list` | Applies a navigation group list inside footer navigation. | `<ul class="footer-nav-group-list"></ul>`
`footer-info` | Applies information area inside footer that contains copyright, legal and contact links. | `<div class="footer-info"></div>`
`footer-info-legal` | Applies legal area inside footer information. | `<div class="footer-info-legal"></div>`
`footer-info-legal-link-list` | Applies a list of links inside footer information legal. Grid component is used for alignment. | `<ul class="footer-info-legal-link-list grid"></ul>`
`footer-info-contact` | Applies a list of contact links inside footer information. Grid component is used for alignment. | `<ul class="footer-info-contact-list grid"></ul>`

### Examples

#### Example 1

The following example shows a footer with a short description, two navigation groups, copyright, links to legal documents and other pages.

```html
<footer class="footer">
  <div class="container">
    <div class="footer-nav">
      <div class="grid grid--gutter grid--gutter--double">
        <div class="grid-col grid-col--1of2 grid-col--small--full">
          <h2>About company</h2>
          <p>Ornare interdum nascetur enim lobortis nunc amet placerat pellentesque nascetur in adipiscing. Interdum amet accumsan placerat commodo ut amet aliquam blandit nunc tempor lobortis nunc non. Mi accumsan. Justo aliquet massa adipiscing cubilia eu accumsan id. Arcu accumsan faucibus vis ultricies adipiscing ornare ut. Mi accumsan. rnare interdum nascetur enim lobortis nunc amet placerat pellentesque. Interdum amet placerat commodo ut amet aliquam blandit nunc tempor lobortis nunc non.</p>
        </div>
        <div class="grid-col grid-col--1of4 grid-col--small--1of2 grid-col--xsmall--full">
          <h2>Navigation</h2>
          <ul class="footer-nav-group-list">
            <li>
              <a href="#">Home</a>
            </li>
            <li>
              <a href="#">Services</a>
            </li>
            <li>
              <a href="#">Products</a>
            </li>
            <li>
              <a href="#">Blog</a>
            </li>
            <li>
              <a href="#">Contact</a>
            </li>
          </ul>
        </div>
        <div class="grid-col grid-col--1of4 grid-col--small--1of2 grid-col--xsmall--full">
          <h2>Help center</h2>
          <ul class="footer-nav-group-list">
            <li>
              <a href="#">Ornare interdum</a>
            </li>
            <li>
              <a href="#">Nascetur enim</a>
            </li>
            <li>
              <a href="#">massa amet</a>
            </li>
            <li>
              <a href="#">Nascetur nunc</a>
            </li>
            <li>
              <a href="#">Nascetur nunc</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <hr />
    <div class="footer-info">
      <div class="footer-info-legal">
        &copy; 2018 My Company. All rights reserved.
        <ul class="footer-info-legal-link-list grid grid--gutter grid--gutter--half grid--uniform">
          <li class="grid-col">
            <a href="#">Terms of service</a>
          </li>
          <li class="grid-col">
            <a href="#">Privacy policy</a>
          </li>
          <li class="grid-col">
            <a href="#">Contact Us</a>
          </li>
        </ul>
      </div>
      <ul class="footer-info-contact-list grid grid--gutter grid--gutter--half grid--uniform">
        <li class="grid-col">
          <a href="#">Link 1</a>
        </li>
        <li class="grid-col">
          <a href="#">Link 2</a>
        </li>
        <li class="grid-col">
          <a href="#">Link 3</a>
        </li>
      </ul>
    </div>
  </div>
</footer>
```
