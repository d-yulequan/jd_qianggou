## 可用于JD抢购

### dist下为windows可执行文件，可直接运行

### 总体步骤如下：

### 第一步：获取cookie
登录pc版JD商城，进入购物车，打开控制台，查看接口https://api.m.jd.com/api?functionId=pcCart_jc_getCurrentCart的cookie，填入cookie的输入框

### 第二步：清空购物车
减少其他店铺因素

### 第三步：获取商品id
找到需要抢购的商品，查看详情，可以看到浏览器的URL为https://item.jd.com/xxxxxxxx.html，复制xxxxxxxx填入商品ID框，

### 第四步：设置抢购时间和数量
抢购时间需要格式设置，格式为yyyy-MM-dd HH:mm:ss，如2021-11-02 12:00:00。数量可随意设置，但需要考虑到店铺的库存以及是否设置为限购1件。

### 第五步：开始抢单
这个时候可以泡一杯茶，静待好事发生。

### v1版与v2版有些许不同，以下会有说明。
v1版的商品会自动加入购物车，原理是调用加入购物车后，商品在购物车中是默认选中状态，然后再调用下单
而v2版是手动加入购物车（这个可以百度下jd如何在预约阶段加车），随后调用购物车全选接口，再调用下单
两者的区别在于加入购物车接口和全选购物车接口的耗时，推荐v2版。

## 战果
本人鞋迷，目前收获一双大三角、一双闪现3
