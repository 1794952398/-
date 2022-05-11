### @RequestBody和@ResponseBody
  `@ReponseBody`作用于方法上，表示该方法的范围结果直接写入httpresponsebody中，一般在异步获取数据时使用（也就是AJAX），在使用`@RequestMapping`后，返回值通常解析为跳转路径，但是加上`@ResponseBody`后，返回结果不会被解析为跳转路径，而是直接写入 HTTP response body中。比如ajax异步获取数据，加上`@ResponseBody`后，会直接返回 json 数据
 ----- ----
`@RequestBody`作用在形参列表上，用于将前台发送过来的 固定格式的数据（xml或者json）数据封装为对应的 Javabean 对象，封装时使用到的一个对象是系统默认配置的

