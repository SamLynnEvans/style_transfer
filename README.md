# style_transfer

Neural style transfer allows the style of one image to be imposed upon the content of another. The technique was first proposed by <a href="https://arxiv.org/abs/1508.06576">Gatys et al</a> and has so far been used to create images in the fashion of particularly stylistic artists.<br><br>
In this method a content image and a style image are put through layers of a pretrained image-identification model (in this case VGG-16). As the layers get deeper, the model begins to pay attention to more abstract and stylistic features of the image. A loss function compares these abstract features obtained from the stye image to the content image, and changes the content image to make it more similar.<br><br>
![content style](https://user-images.githubusercontent.com/28839356/46339495-dccabb80-c62a-11e8-86d2-3a1885bd9786.png)
<br>
<br><br>
After reading the paper, I implementing the model myself. Here's an example outcome with Kaganawa's waves and my github profile picture.
<br><br>
![2j6w69](https://user-images.githubusercontent.com/28839356/46343514-e6a5ec00-c635-11e8-8ed9-69def2578f17.gif)
<br><br>
To use it yourself, run the jupyter notebook, changing PathyStyle to the path to the style image and PathContent to the path of your content image. Change the ratio of how heavily style and content loss are penalised when you call train.
<br><br>
Let me know if you use it, or make any excellent images!
