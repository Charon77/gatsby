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

This document addresses the configuration file for Gatsby, `gatsby-config.js`.

`gatsby-config.js` is used to config stuffs.


# Common Usage
... examples

# Fields
Here lies some fields

## siteMetadata
## pathPrefix
## mapping
## plugins
## polyfill
## proxy
### prefix
### url


