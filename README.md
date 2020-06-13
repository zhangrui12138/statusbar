# statusbar
各种布局的statusbar  显示
 		//add by zhangrui start for liuhai
 		if (PrizeOption.PRIZE_NOTCH_SCREEN) {
             RelativeLayout.LayoutParams layoutParams = (RelativeLayout.LayoutParams) mSettingLayout.getLayoutParams();
 		    int actionbarr_id = (int)getResources().getIdentifier("status_bar_height", "dimen","android");
             layoutParams.topMargin = (int)getResources().getDimensionPixelSize(actionbarr_id);
             mSettingLayout.setLayoutParams(layoutParams);
         }
 		//add by zhangrui end for liuhai
    
     //add by zhangrui start
 			int navigationbarr_id = (int) mContext.getResources().getIdentifier("navigation_bar_height", "dimen","android");
 			int navigationbarHeight = (int)mContext.getResources().getDimensionPixelSize(navigationbarr_id);
 			int marginHeight = mLayoutParams.height - navigationbarHeight * 2;
             FrameLayout.LayoutParams face_lock_textlayoutParams = (FrameLayout.LayoutParams) face_lock_text.getLayoutParams();
             face_lock_textlayoutParams.topMargin = marginHeight;
             face_lock_text.setLayoutParams(face_lock_textlayoutParams);
 			FrameLayout.LayoutParams face_lock_text2layoutParams = (FrameLayout.LayoutParams) face_lock_text2.getLayoutParams();
             face_lock_text2layoutParams.topMargin = marginHeight + Dp2Px(20);
             face_lock_text2.setLayoutParams(face_lock_text2layoutParams);
 			//add by zhangrui end
      
      
      
