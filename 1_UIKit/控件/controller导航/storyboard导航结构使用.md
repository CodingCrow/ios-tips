## uitabbar + navigationController


- 1）删除故事版中默认内容，添加一个uitabbarController 并设置为initial controller
- 2) 将默认的controller删除，添加2个navigationController,按住control拖至uitabbercontroller建立relationship
- 3) 在controller里面bar item 设置title和image，当前选中样式需要到代码里面设置，
例如：self.tabBarItem.selectedImage=[UIImage imageNamed:@"ts探索_sel"];
- 4）建立内容页与navigationController的relationship，用navigationController+control 拖至 内容页的controller

- 5）若某页中不希望出现navigation 和 tabbar ，可以在controller中选择hide button bar on push

代码中设置隐藏：self.hidesBottomBarWhenPushed=YES;  

这个方法要注意使用的位置，在跳转前的控制器中使用，也可以用xxx.hidesBottomBarWhenPushed针对特定控制器
