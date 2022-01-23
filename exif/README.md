# Display pictures with EXIF Metadata

## Purpose

This shortcode will convert `{{<exif src="path/to/picture.jpg" alt="My Picture">}}` into this :

```html
<figure>
<img src="<image permalink>" alt="My Picture">
    <figcaption class="exif"> My Picture
        <br />CameraModel LensModel ApertureValue FocalLength ExposureTime ISOValue
        <br />ArtistName - PictureDateTime - CopyrightLicense
    </figcaption>
{{end }}
</figure>
```

Example :

```golang
{{< exif src="photos/visite-cave-champagne/DSC_0023.jpg" alt="Voûtes taillées dans la craie" >}}
```

Will render :

![exif](exif.png)



## Showcase

- [Visite d'une case de Champagne](https://blog.zedas.fr/posts/visite-cave-champagne/) : The Blog article that made me writing this shortcode

If you want to display your shortcode usage in this showcase, feel free to open au Pull Request on this file or [contact me](https://blog.zedas.fr/contact/)

