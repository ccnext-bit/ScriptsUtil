# ScriptsUtil
一些效率脚本工具集合

### find_unuse_image
查找RN项目里未使用的图片资源node脚本
#####使用步骤
1. 拷贝`find_unuse_image.js`到RN项目根目录
2. 修改`rnRootFilePath`（js代码存放路径）
3. 修改`imgFilePath`(图片资源存储路径)
4. `node find_unuse_image.js`

输出预览

```
$ node find_unuse_image.js 

{
  path: '/Users/CC/Git/rn-app/img/icon_home@2x.png',
  size: '2KB',
  byteSize: 1677
}
{
  path: '/Users/CC/Git/rn-app/ReactNative/Image/icon_cat.png',
  size: '16KB',
  byteSize: 16304
}
...
所有的图片资源数量：1024
使用的图片资源数量：725
未使用的图片资源数量：101
是否删除未使用的图片(yes/no)？yes
删除 /Users/yfw/Git/rn-app/img/icon_home@2x.png
....
共删除了101个文件，总共节省了4M
```


