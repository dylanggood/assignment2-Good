# Dylan Good

One interesting fact about me is that I am an Elden Lord. Not many people know what Elden Lord is, but it is
quite the accoomplishment. I have defeated all of the shardbearers including Starscourge Radahan, and taken their 
great runes. With all of these great runes, I was able to restore the Elden Ring and take my throne.

![image of me](IMG_4671.jpeg)

---

# Tables

We are going to create a table with my favorite cities!

| City Name | Important Locations | Time Spent |
| --- | --- | --- |
| Omaha | Orpheum Theater | 3 hrs |
| St. Louis | Steel Arch | 2 hrs |
| Tampa | Holms Beach | 5 hrs |
| Des Moines | Iowa State Fair | 2 Days |

---

> “The true sign of intelligence is not knowledge but imagination." *Albert Einstein*
> "Believe you can and you're halfway there." *Theodore Roosevelt*

---

> "How to programatically lighten or darken a hex value with JavaScript?"

[stackoverflow.com link](https://stackoverflow.com/questions/5560248/programmatically-lighten-or-darken-a-hex-color-or-rgb-and-blend-colors)

```
function LightenDarkenColor(col, amt) {
  
    var usePound = false;
  
    if (col[0] == "#") {
        col = col.slice(1);
        usePound = true;
    }
 
    var num = parseInt(col,16);
 
    var r = (num >> 16) + amt;
 
    if (r > 255) r = 255;
    else if  (r < 0) r = 0;
 
    var b = ((num >> 8) & 0x00FF) + amt;
 
    if (b > 255) b = 255;
    else if  (b < 0) b = 0;
 
    var g = (num & 0x0000FF) + amt;
 
    if (g > 255) g = 255;
    else if (g < 0) g = 0;
 
    return (usePound?"#":"") + (g | (b << 8) | (r << 16)).toString(16);
  
}
```
[snippet code](https://css-tricks.com/snippets/javascript/lighten-darken-color/)