# SquareImageView

English on the bottom

一个安卓正方形ImgeView控件
使用方式：
1：导入SqueraImageView到您的项目

2：在XML文件中，设置宽度为设定值，高度为任意值
 <yourpackage.SquareImageView
            android:id="@+id/card_image_view"
            android:layout_width="fill_parent"
            android:layout_height="360dp"
            android:scaleType="fitXY" />
            
注释：如果想设置成宽度等于高度
修改下面这个函数即可

    @Override
    protected void onMeasure(int widthMeasureSpec, int heightMeasureSpec) {
    
        //修改成super.onMeasure(heightMeasureSpec, heightMeasureSpec);
        super.onMeasure(widthMeasureSpec, widthMeasureSpec);
    }
This is a squera ImageView On Android

Usage:
1: copy SqueraImageView to your project.
2: setting the width to a value, and height to any value on the XML file

  <yourpackage.SquareImageView
            android:id="@+id/card_image_view"
            android:layout_width="fill_parent"
            android:layout_height="360dp"
            android:scaleType="fitXY" />
  3: If you want to set the weidth eques to the height, just change the function below as the note
    @Override
    protected void onMeasure(int widthMeasureSpec, int heightMeasureSpec) {
    
        //修改成super.onMeasure(heightMeasureSpec, heightMeasureSpec);
        super.onMeasure(widthMeasureSpec, widthMeasureSpec);
    }

