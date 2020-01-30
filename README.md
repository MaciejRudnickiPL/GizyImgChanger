# GizyImgChanger
Changes images between new and old versions with full screen preview.
example:
http://x20.pl/change/

## Getting Started
To work:
### HTML
Add two images with the same dimensions and put in div.
```
   <div class="imgDiv">
        <img  src="img/new.jpg" data-big="bigNew.jpg">>
        <img  src="img/old.jpg" data-big="bigOld.jpg">>
    </div>
 ```  

You can add class to img to set size of image.

```
 <div class="imgDiv">
       <img class="myImg" src="img/new.jpg">
        <img class="myImg" src="img/old.jpg">
 </div>
```

You can add a large size image to the full screen preview.
```
 <div class="imgDiv">
        <img  src="img/new.jpg" data-big="bigNew.jpg">>
        <img  src="img/old.jpg" data-big="bigOld.jpg">>
    </div>
```

### JavaScript

```
import GizyImgChanger from './GizyImgChanger';
new GizyImgChanger('imgDiv').start();
```

#### JavaScript Options
```
  let gic = new GizyImgChanger("divAll");
  gic.settings.imageSize.type = "css";
  gic.settings.fullScrean.full = true;
  gic.settings.fullScrean.type = "full";
  gic.settings.fullScrean.big = false;
```

##### Image changer settings
```
settings.imageSize.type: 
      => "css" - css settings, 
      => "natural" - natural image resolution
      => "set" - resize to settings.imageSize.width and height
settings.imageSize.width:300  => width of image (number)
settings.imageSize.height:400 => height of image (number)
```
##### Full screen image settings  
```
settings.fullScreen.full: 
      => true - double click for fullsreen preview 
      => false - without 
settings.fullScreen.type: 
      => "css" - css settings, 
      => "natural" - natural image resolution
      => "full" - resize to full screen
      => "set" - resize to settings.imageSize.width and height
settings.fullScreen.bigUrl:"/bigImage"  => subdirectory for big image
settings.fullScreen.big: 
      => true - big image in fullscreen preview   
      => false - oryginal image in fullscreen preview  
settings.fullScreen.backColor => background color for fullscreen preview  
```
     
      
## Version
1.1 Works on my computer :) 
## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
