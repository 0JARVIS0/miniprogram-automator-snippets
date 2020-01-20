# miniprogram-automator-snippets

### 小程序自动化SDK API 代码片段

###### 提供以下代码片段：

1. atuomator
  * automator.connect __连接开发者工具__
  * automator.launch __启动并连接开发者工具__
2. miniProgram
  * miniProgram.callWxMethod __调用 wx 对象上的指定方法。调用异步方法时无需传入 success 及 fail 回调函数__
  * miniProgram.currentPage
  * miniProgram.evaluate __往 AppService 注入代码片段并返回执行结果。__
  * miniProgram.exposeFunction __在 AppService 全局暴露方法，供小程序侧调用测试脚本中的方法。__
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
  * miniProgram.remote __开启工具真机调试功能__
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
  * element.attribute __获取的是标签上的值，因此它的返回类型一定是字符串 可以获取到 class 和 id 之类的值，element.property 不行__
  * element.property __可以获取到文档里对应组件列举的大部分属性值，比如表单 input 等组件的 value 值__
  * element.wxml __获取元素wxml__
  * element.outerWxml __获取元素本身wxml__
  * element.value
  * element.style
  * element.tap
  * element.longpress
  * element.touchstart __触摸事件__
  * element.touchmove
  * element.touchend
  * element.trigger __触发元素事件。type: 事件名，detail: 传递值__
  * element.input __触发输入，仅input与textarea有效__
  * element.callMethod __调用组件实例指定方法，仅自定义组件可以使用。同miniProgram.callWxMethod__
  * element.data __获取组件实例渲染数据，仅自定义组件可以使用。path: 数据路径__
  * element.setData __设置组件实例渲染数据，仅自定义组件可以使用。data: 要改变的数据__
  * element.callContextMethod __调用上下文Context 对象方法，仅 video 组件可以使用。__
  * element.scrollWidth __仅scroll-view使用__
  * element.scrollHeigh __仅scroll-view使用__
  * element.scrollTo __仅scroll-view使用__
  * element.swipeTo __仅swiper使用__
  * element.moveTo __仅movable-view使用__
  * element.slideTo __仅slider使用__

###### 除了小程序sdk外，还提供了以下jest相关代码片段，方便书写
  * describe
  * beforeAll
  * afterAll
  * beforeEach
  * afterEach
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