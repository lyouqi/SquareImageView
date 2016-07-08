# SquareImageView
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
