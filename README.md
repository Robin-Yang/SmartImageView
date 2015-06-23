# SmartImageView
很好用的开源框架，主要应用于Android的网络图片加载，如请求新闻客户端的图片加载。

使用步骤：

 1.直接com的包复制到项目当中

 2. 在布局页面使用此控件：必须使用包名.类名这样的全路径，否则无法找到
 3. 
 
<!-- 引入第三方控件用于显示图片 -->
<com.loopj.android.image.SmartImageView
  android:id="@+id/iv"
  android:layout_height="70dp"
  android:layout_width="70dp"
  android:contentDescription="news"
  />


调用 setImageUrl,将图片的网络地址赋值给控件即可

//实例化 SmartImageView 对象
SmartImageView imageView =
(SmartImageView)convertView.findViewById(R.id.iv);
//给 SmartImageView 设置一个图像的 URL 则 SmartImageView 会自动加载图片
imageView.setImageUrl(news.getImage());
