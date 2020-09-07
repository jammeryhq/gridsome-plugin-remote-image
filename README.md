<div align="center">

<a href="https://www.jammeryhq.com" title="JammeryHQ" target="_blank">

  <img src="./jammeryhq.png" width="128" />
  
</a>

<p>
Fast-track your JAMstack development & learning
</p>
</div>

<hr />

# About this plugin

Simple plugin to download remote images in Gridsome, which enables you to take advantage of Gridsome's native image resizing and optimisation.

## Installation

```bash
npm install @jammeryhq/gridsome-plugin-remote-images

# or

yarn add @jammeryhq/gridsome-plugin-remote-images
```

## Key features

* Download one image ( String field )
* Download multiple images ( Array fields )
* Caching
* Option to keep the original field value

## How to use

```js
//gridsome.config.js

module.exports = {
  siteName: 'Gridsome',
  plugins: [
    //...
    {
      use: '@jammeryhq/gridsome-plugin-remote-images',
      options: {
        'typeName' : 'Entry',
        'sourceField': 'remoteImage',
        'targetField': 'imageDownloaded',
        'targetPath': './src/assets/remoteImages'
      }
    },
    {
      use: '@jammeryhq/gridsome-plugin-remote-images',
      options: {
        'typeName' : 'Entry',
        'sourceField': 'remoteImages',
        'targetField': 'imagesDownloaded',
        'targetPath': './src/assets/remoteImages'
      }
    }
  ]
  //...
}
```

## Documentation

You can find the complete documentation here: https://webstone.info/documentation/gridsome-plugin-remote-image
