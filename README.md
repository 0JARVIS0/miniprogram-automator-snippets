# miniprogram-automator-snippets

### 小程序自动化SDK API 代码片段

#### 提供以下代码片段：
1. atuomator
    * automator.connect          _连接开发者工具_
    * automator.launch          _启动并连接开发者工具_

2. miniProgram
    * miniProgram.callWxMethod          _调用 wx 对象上的指定方法。调用异步方法时无需传入 success 及 fail 回调函数_
    * miniProgram.currentPage
    * miniProgram.evaluate          _往 AppService 注入代码片段并返回执行结果。_
    * miniProgram.exposeFunction          _在 AppService 全局暴露方法，供小程序侧调用测试脚本中的方法。_
    * miniProgram.mockWxMethod
    * miniProgram.navigateBack
    * miniProgram.navigateTo
    * miniProgram.pageScrollTo
    * miniProgram.pageStack
    * miniProgram.reLaunch
    * miniProgram.redirectTo
    * miniProgram.restoreWxMethod
    * miniProgram.switchTab
    * miniProgram.systemInfo
    * miniProgram.close
    * miniProgram.disconnect
    * miniProgram.remote          _开启工具真机调试功能_

3. page
    * page.path
    * page.query
    * page.size
    * page.scrollTop
    * page.$
    * page.$$
    * page.waitFor
    * page.data
    * page.setData
    * page.callMethod
    
4. element (支持驼峰格式默认组件名和额外的customComponent)
    * element.tagName
    * element.$
    * element.$$
    * element.size
    * element.offset
    * element.text
    * element.attribute          _获取的是标签上的值，因此它的返回类型一定是字符串_
                                 _可以获取到 class 和 id 之类的值，element.property 不行_
    * element.property          _可以获取到文档里对应组件列举的大部分属性值，比如表单 input 等组件的 value 值_
    * element.wxml          _获取元素wxml_
    * element.outerWxml          _获取元素本身wxml_
    * element.value
    * element.style
    * element.tap
    * element.longpress
    * element.touchstart          _触摸事件_
    * element.touchmove
    * element.touchend
    * element.trigger          _触发元素事件。type: 事件名，detail: 传递值_
    * element.input          _触发输入，仅input与textarea有效_
    * element.callMethod          _调用组件实例指定方法，仅自定义组件可以使用。同miniProgram.callWxMethod_
    * element.data          _获取组件实例渲染数据，仅自定义组件可以使用。path: 数据路径_
    * element.setData          _设置组件实例渲染数据，仅自定义组件可以使用。data: 要改变的数据_
    * element.callContextMethod          _调用上下文Context 对象方法，仅 video 组件可以使用。_
    * element.scrollWidth          _仅scroll-view使用_
    * element.scrollHeigh          _仅scroll-view使用_
    * element.scrollTo          _仅scroll-view使用_
    * element.swipeTo          _仅swiper使用_
    * element.moveTo          _仅movable-view使用_
    * element.slideTo          _仅slider使用_

详细文档可查阅[微信小程序自动化](https://developers.weixin.qq.com/miniprogram/dev/devtools/auto/ "微信小程序自动化")官方文档

--------------------------------------------------------------------------------------------------------------

#### 除了小程序sdk外，还提供了以下jest相关代码片段，方便书写

  * describe
  * beforeAll
  * afterAll
  * beforeEach
  * afterEach
  * test
  * expect.toBe
  * expect.not.toBe
  * expect.toEqual
  * expect.not.toEqual
  * expect.toBeCloseTo
  * expect.toBeNull
  * expect.not.toBeNull
  * expect.toBeDefind
  * expect.toBeUndefined
  * expect.toBeNaN
  * expect.toBeTruthy
  * expect.toBeFalsy

  更详细的用法也可以参考[jest官方文档](https://jestjs.io/docs/zh-Hans/getting-started "jest官方文档")