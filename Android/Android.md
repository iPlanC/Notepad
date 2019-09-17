# Android 开发笔记

## Android 介绍
- 基于事件

## Android 工程结构
```
\src								//源码目录
\gen								//自动生成的资源目录文件
\Android							//Android 虚拟机目录
\Assists							//媒体文件（？）
\res								//资源目录
	\drawable						//多媒体库
	\layout							//界面目录
		\main.xml					//界面文档
		......
	\values							//存储公共值的目录
Androidmanidfest.xml				//安装.apk时需要的配置文件
default.properties
progrard.cfg
```

## Android ID 使用
	//创建一个ID
	@+id/...
	//引用一个ID
	@id
	
	//将ID:"abc"赋予控件
	android:id="@+id/abc"
	
## Android 控件实例化及设置监听器
	//控件实例化
	[public/private] (控件类) (名称) = (控件类)findViewById(R.id.(控件ID));
	
	//按钮设置监听器
	(按钮).setOnClickListener(new OnclickLisenter {
		public void onClick(view v) {
		}
	});
