# FloatWindows
1. 悬浮窗控制在输入法之下
WindowManager mWindowManager = (WindowManager) applicationContext.getSystemService(Context.WINDOW_SERVICE);
WindowManager.LayoutParams mLayoutParams = new WindowManager.LayoutParams();
mLayoutParams.flags = WindowManager.LayoutParams.FLAG_NOT_FOCUSABLE | WindowManager.LayoutParams.FLAG_ALT_FOCUSABLE_IM;

2. Toast悬浮窗
mLayoutParams.type = WindowManager.LayoutParams.TYPE_TOAST;
