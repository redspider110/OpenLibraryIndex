# OpenLibraryIndex
OpenLibraryIndex

## 图片加载库  
4 大图片加载库  
- [UIL](https://github.com/nostra13/Android-Universal-Image-Loader)  
已经不再维护。老牌加载库，实现了很多基本经典的功能。  
- [Picasso](https://github.com/square/picasso)  
`Square` 公司开源的图片加载框架，简单易用。大小只有 `100` k，方法数也很少，只会缓存原始尺寸的图片。  
- [Glide](https://github.com/bumptech/glide)  
`Google` 一位员工的大作，完全是基于 `Picasso` 并沿袭了它的简洁风格，但是在此做了大量优化与改进。默认的 `Bitmap` 格式是 `RGB_565` 格式，而 `Picasso` 默认的是 `ARGB_8888` 格式，这个内存开销要小一半。`Glide` 会根据 `ImageView` 来缓存相应大小的图片尺寸，而不是加载图片原始大小。最重要的一个特性是 `Glide` 支持加载 `Gif` 动态图，而 `Picasso` 不支持该特性。  
- [Fresco](https://github.com/facebook/fresco)  
 `Facebook` 出品的新一代的图片加载库，将图片放到一个特别的内存区域叫 `Ashmem` 区，属于 `Native` 堆，图片将不再占用 `App` 的内存，并不在 `Java` 层处理，能大大的减少 `OOM` 。   
