# cordova-plugin-facerecognition
百度人脸活体检测插件

# 支持平台
1. android 

## How to use?
```js
  /**
   * 参数 数组 []   传入自定义动作,数组顺序即为动作顺序，可传空数组,默认[1,0,2,3]
   * 0 眨眼 1 张嘴 2 向左转头 3 向右转头 4 向左或者向右转头 5 抬头 6 点头
   * success--->  图片数组(有引号包裹，可能需要自己截取) 
   * 图片尽可能不要截取转头和点头的照片，会比较模糊
   * err---> 0 取消操作 -1 等待时间过长或其他检测错误   -2 没有访问照相机权限
   */
window.cordova.exec(success => {
  }, err => {
  }, 'BDFaceVerify', 'FaceCoolMethod', [])
```

## 需要在百度人脸活体检测注册app，项目签名与百度注册的app保持一致
