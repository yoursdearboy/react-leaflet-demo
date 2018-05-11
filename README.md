# Demo for issue [react-leaflet-demo#255](https://github.com/PaulLeCam/react-leaflet/issues/255)

See [commits](https://github.com/yoursdearboy/react-leaflet-demo/commits/master) messages for errors and diffs for solutions.

For the second issue note file names:

```
2273e3d8ad9264b7daa5bdbf8e6b47f8.png%22)marker-icon-2x.png
2273e3d8ad9264b7daa5bdbf8e6b47f8.png%22)marker-shadow.png
```

Here are two errors:

1. File name must be just [hash].[ext] (e.g. `2273e3d8ad9264b7daa5bdbf8e6b47f8.png`)
2. These hashes are calculated for `marker-icon.png` file

Somehow using hash in name breaks it.
To avoid this we can change name template in file-loader.
But [it is important](https://survivejs.com/webpack/optimizing/adding-hashes-to-filenames/) feature, that must be turned on for production.

- [ ] Find a way to get hash back
