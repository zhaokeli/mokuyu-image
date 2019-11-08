# mokuyu-image
引类是引用thinkphp中的图片处理类,文档可以参考 [图片处理手册](https://www.kancloud.cn/manual/thinkphp5_1/354123)
##添加水印
```
$src_img='1.png';
$water_img='sy.png';
$dest_img='2.png';
//打开源图片
$imgobj  = \mokuyu\Image::open($src_img);
//添加水印
//$pos位置，详细请查看类内常量
//80为透明度
$imgobj->water($water_img, $pos, 80)->save($dest_img);
```