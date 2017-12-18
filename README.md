## setState()函数在任何情况下都会导致组件重渲染吗？如果setState()中参数还是原来没有发生任何变化的state呢
setState都会导致组件重新渲染，即使所以需要  shouldComponentUpdate(nextProps,nextState){}，判断State是否发生变化
## 如果组件的state没有变化，并且从父组件接受的props也没有变化，那它就一定不会重渲染吗？
会的，父组件刷新会带动子组件刷新，shouldComponentUpdate(nextProps,nextState){}进行判断，进行处理
