# GizyImgChanger
Changes images between new and old versions.


## Getting Started
To work:
### HTML
Add two images with the same dimensions and put in div.
```
   <div class="imgDiv">
        <img  src="{{ asset('img/new.jpg') }}">
        <img  src="{{ asset('img/old.jpg') }}">
    </div>
 ```  
You can add many divs witch imgClass and two images.
You can add class to img to set size of image.
```html
 <div class="imgDiv">
        <img class="imgClass" src="{{ asset('img/new.jpg') }}">
        <img class="imgClass" src="{{ asset('img/old.jpg') }}">
 </div>
```
### JavaScript
```
new GizyImgChanger('imgDiv').start();
```

## Version
1.0 Works on my computer :) 
## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
