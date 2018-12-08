# HOW TO USE

```

class MY_Loader extends CI_Loader {
	use codeigniter_packages_loader;


}

```

# codeigniter-view

加载视图库的时候，视图库仅仅是作为常用的视图文件，不要试图希望加载一个试图库就能解决整个项目的视图
codeigniter-view仅仅应该包含tmpl,与html片段

比如一个视图提供bootstrap中media-list样式，该视图文件就只需要包含一个media-list的html片段，当然也可以是自己基于media-list修改后的视图
这样当该视图被重复使用的时候，可以加快开发速度，但它的存在应该仅仅是为了前期快速出原型，到最后成型的时候，该view的片段应该融于项目中

视图的主要js代码应该在项目中，而不是在codeigniter-view中

