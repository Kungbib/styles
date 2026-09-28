# kungbib/styles
Bootstrap theme for use in development at the National Library of Sweden.

The theme is based on Bootstrap 5.3.

See [Bootstrap documentation](https://getbootstrap.com/docs/5.3/getting-started/introduction/) on how to use Bootstrap components.

Also see [KB Styleguide](https://styleguide.kb.se) for brand guidelines.

# Usage
The are several ways to consume this package.

## Installation

## NPM package
Install the NPM package if you want all the benefits of NPM, and want to customize the theme:

`$ npm install @kungbib/bootstrap-styles`

Here you have several options:

1. Use the compiled css file:

```
<link rel="stylesheet" href="node_modules/@kungbib/bootstrap-styles/lib/css/theme.css">
```

2. Use Sass file, if your project supports it:

```
<link rel="stylesheet" href="node_modules/@kungbib/bootstrap-styles/lib/scss/theme.css">
```

3. Use Sass files combined with your own variables, if you want to customize the theme:

```
// The order of these imports are important.
// Project specific styles following
// Any bootstrap variables should be imported before importing bootstrap package

// Your own variables 
@import 'variables';
// Kungbib-styles variables
@import 'node_modules/@kungbib/bootstrap-styles/lib/scss/variables';
// Bootstrap import
@import 'node_modules/bootstrap/scss/bootstrap';
// Kungbib-styles styles
@import 'node_modules/@kungbib/bootstrap-styles/lib/scss/styles';

// Icons, optional import 
@import url("https://cdn.kb.se/bootstrap-icons@1.13.1/bootstrap-icons.min.css");

``` 

## Compiled CSS file
If your project does not support NPM packages or SASS files,
[download the code as .zip](https://github.com/Kungbib/styles/archive/refs/heads/master.zip), then use the `lib/css/theme.css` file as-is:

```
<link rel="stylesheet" href="theme.css">
```


## Contributions

Please leave comments/issues about 3.x in this repo.  
Everything regarding 1.x should be handled in the [frontend-guide repo](https://github.com/Kungbib/frontend-guide).
