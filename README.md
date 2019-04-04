# Photo Viewer  
> This plugin is intended to show a picture from an URL into a Photo Viewer with zoom features.

## How to Install

Cordova:
```bash
cordova plugin add https://github.com/HouseCool/cordova.HouseCoolPlugins.photoviewer.git
```

Ionic 2:
```bash
$ ionic cordova plugin add com-sarriaroman-photoviewer
$ npm install --save @ionic-native/photo-viewer
```

### Android
> Out of the box

### iOS
> Out of the box


### API-IOS

#### Show an image

```
PhotoViewer.show('http://my_site.com/my_image.jpg', 'Optional Title');
```

Optionally you can pass third parameter option as object.

Options:
* share: Image download function.

##### Usage

```
var options = {
    share: true, // default is false
};

PhotoViewer.show('http://my_site.com/my_image.jpg', 'Optional Title', options);
```
### API-Android

URL:
* title: Picture captions [mandatory]
* description : Picture description [optional]
* url: Picture address 

```
function Transfer(){
    var url = [
        {"title":"图像1","description"："图片描述","url":"https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=1982513715,1507401127&fm=26&gp=0.jpg"},
    ]
    var options = {
        share: false, // default is false
    };
    PhotoViewer.showMultiple(url,3,options);
}
```


