---
title: "Gatsby Configuration"
---

```javascript
export const gatsbyConfigSchema = Joi.object().keys({
  polyfill: Joi.boolean(),
  siteMetadata: Joi.object(),
  pathPrefix: Joi.string(),
  mapping: Joi.object(),
  plugins: Joi.array(),
  proxy: Joi.object().keys({
    prefix: Joi.string().required(),
    url: Joi.string().required(),
  }),
})
```

`gatsby-config.js` is the configuration file for setting up Gatsby. This sets up 


# Common Usage
... examples

# Fields
Here lies some fields

## siteMetadata

siteMetadata: (object)

Something you can access from every page.

if your siteMetadata is like this:

```javascript
{
  siteMetadata: {
    siteName: "Site Name here"
  }
}
```

you can access `siteName` by using `this.props.data.site.siteMetadata.siteName` in your page.

## pathPrefix

pathPrefix: (string)

Check this out: gatsby/examples/using-path-prefix/

Adds prefix to the site served using Gatsby.

## mapping

Doesn't appear to be used

However, this might be a nice ref.

Check this out: gatsby/examples/using-path-prefix/

## plugins
## polyfill

polyfill: (bool)

Will run `require('core-js/modules/es6.promise')`

## proxy
### prefix
### url


