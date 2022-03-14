# Index about assignment1
### Motivation
* Boji is **super cute**.
* I would like to expression my angry *without things getting awkward*.


### The origin image
![Click here](https://www.bing.com/images/search?view=detailV2&ccid=TLuk40BM&id=5F6BDAEE54503DD3C8EB162EC5A7032496240266&thid=OIP.TLuk40BM2aHvkleWwzdoEgHaEK&mediaurl=https%3a%2f%2fth.bing.com%2fth%2fid%2fR.4cbba4e3404cd9a1ef925796c3376812%3frik%3dZgIkliQDp8UuFg%26riu%3dhttp%253a%252f%252fimg.lemeitu.com%252fm00%252fe6%252fec%252f794d12369e5099511e6b12af0751e646__w.jpg%26ehk%3dFHv7s7%252b99g2YYjZXKim3pKyNny3udyqTnn0b9GcSl%252fQ%253d%26risl%3d%26pid%3dImgRaw%26r%3d0&exph=540&expw=960&q=%e6%b3%a2%e5%90%89&simid=608048252747412627&FORM=IRPRST&ck=AF8A332636CCBB1B991395825D0C05A5&selectedIndex=11)



### The new iamge
![](my_meme.png)


### Code
I used r code like:
<br>

```
library(magick)
image1 <- image_read("boji.jpeg")
image2 <- image_blank(width =474,height=20,color='white') %>%
  image_annotate(text = 'I am going to explode!',size = 20, gravity = "center")
new_image<-image_append(c(image1,image2),stack=TRUE)
image_write(new_image,'my_meme.png')
```
