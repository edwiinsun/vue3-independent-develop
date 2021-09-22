## Vue3 实战项目

-  Vue3的亮点

  - Performance(比vue2 runtime快2倍)

  - Tree shaking  (按需编译代码)
    - 按需打包

  - Ts support  (更优秀的Ts支持)
  - fragment  不在限于模板中单个根节点

  - Composition API (组合API)

  - ![image-20210923020228266](C:\Users\sdsun\AppData\Roaming\Typora\typora-user-images\image-20210923020228266.png)

    ```vue
    在此之前使用的是
    options API: 
    
    export default {
      name: 'HelloWorld',
      props: {
        msg: String,
      },
      data() {},
      methods: {},
    }
    
    Composition API:
    import { onMounted } from 'vue'
    
    function test() {
      onMounted(() => {
        console.log('mounted')
      })
    }
    
    export default {
      name: 'HelloWorld',
      props: {
        msg: String,
      },
      setup() {
        test()    //调用函数
      },
      data() {},
    }
    ```

    - 灵活的逻辑组合与复用

    - 响应式对象

      - ref

      - reactive

    - 生命周期

      - onMounted

      - onUnmounted

  - Custom  Renderer API (组合API)

    - 解决什么问题?       允许用户可以自定义渲染平台

    ```vue
    
    ```

    

  - 内置新特性组件

  