
# TopClear Theme

TopClear is a modern, responsive, and highly customizable theme designed for Salla stores. Built with the latest web technologies, TopClear offers a clean and elegant user experience, making it ideal for merchants who want their online store to stand out.

## Features

- Sleek, modern design with a focus on usability and accessibility
- Fully responsive layout for seamless shopping on any device
- Modular component system for easy customization and scalability
- Built with Twig, SCSS, and ES6 JavaScript for maintainability
- Integrated with Salla's Twilight engine for advanced theme options
- Ready-to-use components for home, product, cart, testimonials, and more
- RTL and LTR support for multilingual stores

## Getting Started

1. Clone or download this repository.
2. Install dependencies with your preferred package manager (e.g., `pnpm install`).
3. Use the provided build tools to compile assets and start development.
4. Customize components and styles in the `src/` and `views/` directories.
5. Follow Salla's documentation to package and publish your theme.

## Directory Structure

- `src/` — Source assets (styles, JS, images)
- `views/` — Twig templates for layouts, pages, and components
- `public/` — Compiled assets for production
- `locales/` — Translation files

## Author

Fayad Adel

---

TopClear is the perfect starting point for building a beautiful, high-performance Salla store. Enjoy modern e-commerce development!

### Prerequisite  
- Basic understanding of HTML, CSS, JS, and the [Twig Template Engine](https://twig.symfony.com/).
- Partner account at [Salla Partners Portal](https://salla.partners/) to create a demo store to publish and test your theme.
- A [Github](https://github.com) account into which the theme can be synced.
- Installing [Salla CLI](https://www.npmjs.com/package/@salla.sa/cli)

### Install  
Theme Raed gets installed by default upon installing the Twilight Themes. Twilight can be installed in two ways:

- Through the [Salla Partners Portal](https://docs.salla.dev/doc-421877/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM#creating-theme-via-salla-partners-portal)

- Through the [Salla CLI](https://docs.salla.dev/doc-422775/?nav=01HNA8QHCPJTCY5VSEZ616JCAK).

Either way, it will trigger the installation of the Twilight Engine and the Theme Raed.  This a complete article for how to [install and create](https://docs.salla.dev/doc-421877/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM) the Twilight Themes.

<p align="right">(<a href="#top">back to top</a>)</p>

## Usage 
Theme Raed will be installed as the default theme when you install Twilight. We'll look at how this theme's directories are set up and how to use the preview mode in the next section.

### Directory structure  
**Theme Raed** is a collection of files and folders that define the Salla Store presentation layer. Following is the directory structure for this starter theme.
```shell
+---scr
    +---assets
    |   +---images      
    |   +---js      
    |   +---styles         
    +---locales
    |       ar.json
    |       en.json
    +---views
        +---components
        |   +---footer
        |   +---header
        |   +---home
        |   +---product
        |   comments.twig
        +---layouts
        |       master.twig
        +---pages
            |   cart.twig
            |   index.twig
            |   loyalty.twig
            |   page-single.twig
            |   thank-you.twig
            +---blog
            |       index.twig
            |       single.twig 
            +---brands
            |       index.twig
            |       single.twig 
            +---customer
               |   notifications.twig
               |   profile.twig
               |   wishlist.twig
               +---orders
               |      index.twig
               |      single.twig
            +---partials
                |   single-comment.twig
                +---product
                  |   card-full-image.twig
                  |   card-mini.twig
                  |   card.twig
                  |   options.twig
                  |   slider.twig
            +---product
            |       index.twig
            |       single.twig
```

### Theme Preview  
Usin [Salla CLI](https://github.com/SallaApp/Salla-CLI), the developer can preview the theme as they are being developed.  The `preview` command helps the developer to get a look at the theme in live mode.

<!-- theme: info -->
> To run the preview command, the developer must be in the theme's root folder.

The developer can run the command `preview` and specify the configuration to view the theme:

```shell title = "Terminal"
salla theme preview

# Alias command for preview
salla theme p
```

On the other hand, the [Partners Portal]() lists the demo stores of the developer. The developer may select a demo store where the theme will be installed, after which the store will be instantly shown in the browser. This is a fantastic option for developers who want to see live updates to their themes appearing on the store right away.

<p align="right">(<a href="#top">back to top</a>)</p>

## Main Features 
By default, Theme Raed home page displays a collection of Pre-Defined and Custom Components. These components are located in the [`src/views/components/home/`](https://github.com/SallaApp/theme-raed/tree/master/src/views/components/home) folder.


### Theme Features  
 Pre-Defined  Components, which are know as Theme Features, listed in the [twilight.json](https://github.com/SallaApp/theme-raed/blob/master/twilight.json) under the `features` section. Below is a list of these components.
 
 | <div style="width:220px">Component</div>                                                       | Discription                                                                                                                                                                 |
 | ---------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | [Youtube](https://docs.salla.dev/doc-422582/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM)                   | This component is responsible for displaying Youtube videos that the developer preselects.                                                                                  |
 | [Fixed Banner](https://docs.salla.dev/doc-422583/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM)              | Fixed banner is the area in charge of displaying a banner that is fixated on the home page.                                                                                 |
 | [Testimonials](https://docs.salla.dev/doc-422584/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM)              | This component displays testimonials that the developer preselects.                                                                                                         |
 | [Parallax backgorund](https://docs.salla.dev/doc-422585/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM)       | This component displays products with a backgournd that zooms out slowly giving a 2D effect.                                                                                |
 | [Photos slider](https://docs.salla.dev/doc-422586/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM)             | Photos are displayed in a slider by using this component.                                                                                                                   |
 | [Store Features](https://docs.salla.dev/doc-422587/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM)            | This component is responsible for showcasing the store features such as a detailed product description, customer reviews of the product, and a fast guest check-out option. |
 | [Square photos](https://docs.salla.dev/doc-422588/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM)             | Use this component to display photos in a square shape.                                                                                                                     |
 | [Fixed products](https://docs.salla.dev/doc-422589/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM)            | Use this component to pin the products that you wish to have displayed always.                                                                                              |
 | [Products slider](https://docs.salla.dev/doc-422590/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM)           | This slider component helps navigate between products vertically/horizontally.                                                                                              |
 | [Featured prodcuts style 1](https://docs.salla.dev/doc-422591/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM) | Using this component, featured products are exhibited in a pre-defined style.                                                                                               |
 | [Featured prodcuts style 2](https://docs.salla.dev/doc-422592/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM) | Using this component, featured products are exhibited in a pre-defined style.                                                                                               |
 | [Featured prodcuts style 3](https://docs.salla.dev/doc-422593/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM) | Using this component, featured products are exhibited in a pre-defined style.                                                                                               |
 | [Latest Products](https://docs.salla.dev/doc-422599/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM)           | This component displays the latest products added to the store automatically.                                                                                               |
 | [Vertical menu with slider](https://docs.salla.dev/doc-422600/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM) | Used to display a menu for a group of the sub-pages' links in a vertical menu.                                                                                              |

### Theme Components
The Custom Components can be easily modified by the developer. They are known as Theme Components. Below is the list of the Custom Components that are shipped by default along with Theme Raed.

| Components                                                                                       | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| [Brands](https://docs.salla.dev/doc-422594/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM)                      | Brands' logos of the store are displayed in this component section.                              |
| [Enhanced Squared Image](https://docs.salla.dev/doc-422595/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM)      | Enhanced images in a square shape are displayed with the help of this component.                 |
| [Main links](https://docs.salla.dev/doc-422596/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM)                  | This component helps to portray the store main links.                                            |
| [Enhanced Slider](https://docs.salla.dev/doc-422597/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM)             | The slider component helps navigate vertically/horizontally.                                     |
| [Slider products with header](https://docs.salla.dev/doc-422598/?nav=01HNFTD5Y5ESFQS3P9MJ0721VM) | Slider products with header displays the products in a slide and give the sldier a header title. |


## Support

The team is always here to help you. Happen to face an issue? Want to report a bug? You can submit one here on Github using the [Issue Tracker](https://github.com/SallaApp/theme-raed/issues/new). If you still have any questions, please contact us via the [Telegram Bot](https://t.me/SallaSupportBot) or join in the Global Developer Community on [Telegram](https://t.me/salladev).

<p align="right">(<a href="#top">back to top</a>)</p>

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create.
Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request.
You can also simply open an issue with the tag "enhancement". Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>

## Credits
- [Salla](https://github.com/sallaApp)
- [All Contributors](../../contributors)
<p align="right">(<a href="#top">back to top</a>)</p>

## License
The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
<p align="right">(<a href="#top">back to top</a>)</p>
