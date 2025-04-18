# Black Background
for darker background
tweaks css like
```css
.box{
   background:rgba(255, 255, 255, 0.01); // opacity
   border-image-source: linear-gradient(135deg, #373737 0%, rgba(255, 255, 255, 0) 100%); // color

}
```
box background alpha value matters lower for black backgrounds
also if border look werid then change it color if white then may #fff if black playaround to find whatever suits

```
.overlay{
    filter: url(#noise) contrast(10%) brightness(120%) opacity(0.16); //opacity
}
```
playaround with opacity low it for darker blacker backgrounds

![image](https://github.com/user-attachments/assets/4a5522ce-7ee2-4d0d-b676-f98cca79f9d7)

here css of this
```
.box{
  padding:2rem;
  height:400px;
  width:800px;
  -webkit-backdrop-filter: blur(5px);
  backdrop-filter: blur(5px);
  background:rgba(255, 255, 255, 0.01);
  box-shadow: 0 4px 32px rgba(0, 0, 0, .2);
  position:relative;
  border-radius:1rem;
  border: 1.5px solid ;
  border-image-source: linear-gradient(135deg, #373737 0%, rgba(255, 255, 255, 0) 100%);
}
.overlay{
  position:absolute;
  height:100%;
  width:100%;
  background:Red;
  top:0;
  left:0;
 filter: url(#noise) contrast(10%) brightness(120%) opacity(0.16);
 clip-path: inset(0 0 0 0 round 1rem); /* Border Radius but for svg*/
}
```
