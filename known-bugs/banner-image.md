	// Current Banner Image Snippet -- Problems setting backrgound Image
```
    var postBannerImage = $('.custom-banner .hs-featured-image-wrapper img').attr('src');  
    $('.custom-banner').css('background-image', 'url(' +postBannerImage + ')');
    $('.custom-banner .hs-featured-image-wrapper img').remove(); 
```

```
    // Background Image With Debugger
 		var postBannerImage = $('.custom-banner .hs-featured-image-wrapper img').attr('src');  
    console.log("postBannerImage: ", postBannerImage);
    console.log(typeof postBannerImage);
    $('.custom-banner').css('background-image', 'url(' +postBannerImage + ')');
    $('.custom-banner .hs-featured-image-wrapper img').remove(); 
```

```
    // Current fix given conflicting URL Encoding 
    var postBannerImage = $('.custom-banner .hs-featured-image-wrapper img').attr('src');  
    $('.custom-banner').css('background-image', "url(\"" +postBannerImage + "\")");
    $('.custom-banner .hs-featured-image-wrapper img').remove(); 
```

```
 $('.bgimg-main1').each(function() {
        var imgSrc = $(this).find('img').attr('src');
        $(this).css('background-image', 'url("' + imgSrc + '")');
    });
```
