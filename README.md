# Edition with i18n

The newsletter theme for [Ghost](http://github.com/tryghost/ghost/). This is the latest development version of Edition! If you're just looking to download the latest release, download the theme [here](https://github.com/TryGhost/Edition/archive/refs/heads/main.zip).

#### This fork based on last master of 08/03/2022 supports both French and English locales
##### Feature added: Integration with commenting system [Isso](https://github.com/posativ/isso) and [Ghost Portal](https://github.com/TryGhost/Portal) for newsletters/memberships

One showstopper with Ghost Portal: [lack of i18n support](https://github.com/TryGhost/Portal/pull/119).

# Development

Edition styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
# Install
yarn

# Run build & watch for changes
$ yarn dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

```bash
# create .zip file
yarn zip
```

# PostCSS Features Used

- Autoprefixer - Don't worry about writing browser prefixes of any kind, it's all done automatically with support for the latest 2 major versions of every browser.

# Copyright & License

Copyright (c) 2013-2022 Ghost Foundation - Released under the [MIT license](LICENSE).
