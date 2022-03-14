# Index about assignment1
### Motivation
* Boji is **super cute**.
* I would like to expression my angry *without things getting awkward*.


### The origin image
![Click here](https://th.bing.com/th/id/R.4cbba4e3404cd9a1ef925796c3376812?rik=ZgIkliQDp8UuFg&riu=http%3a%2f%2fimg.lemeitu.com%2fm00%2fe6%2fec%2f794d12369e5099511e6b12af0751e646__w.jpg&ehk=FHv7s7%2b99g2YYjZXKim3pKyNny3udyqTnn0b9GcSl%2fQ%3d&risl=&pid=ImgRaw&r=0)



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
