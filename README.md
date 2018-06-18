# MATLAB to Dash Docset

Convert MATLAB Help Document to Docset for Dash.app to use.

![image](https://user-images.githubusercontent.com/13360124/32131274-a56a475e-bbdc-11e7-81e0-c17ed5be342a.png)

## How to Use?

Open our [releases page](https://github.com/acbetter/matlab2dash/releases) and download the [binary file (about 10 MB)](https://github.com/acbetter/matlab2dash/releases/download/v1.1/matlab2docset).

Then open `Termainal.app` and input this command:

```shell
chmod +x matlab2docset && ./matlab2docset
```

Please wait for a minutes...

[![asciicast](https://asciinema.org/a/187621.png)](https://asciinema.org/a/187621)

The script will auto find the `MATLAB.app` which was installed in your computer and create the docset file in your `~/Downloads` directory. The size of the docset file will be about 1.6 GB, so please wait it.

Why 1.6 GB? Because of the new verison Dash doesn't support `os.symlink` feature, so I can't use system link to link the docset. So the docset file copy all the `MATLAB.app` help documents which is about 1.6 GB...

## Contact && Bugs Report

Please post bugs and issues on [github](https://github.com/acbetter/matlab2docset/issues). Thank you!

## LICENSE

MIT.

## 中文简介

本程序可以把 `MATLAB.app `自带的帮助文档转换成 `Dash.app` 可以使用的文档。
