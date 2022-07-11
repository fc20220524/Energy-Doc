# Energy-Doc

## 文档地址
```
http://23.225.148.194:2888/dev-api/doc.html
```

## 已完成接口
- [x] 【用户信息、我的团队】接口  /api/rebate/querymyteamdata、/api/getInfo、/api/register新增用户昵称字段，前端需把username改为nickName
- [x] 【持有收益时间轴】接口  /api/product/hold/logPageList/{holdId} 新增收益金额字段（money）
- [x] 【官方群聊】接口  /ucenter/groupInfo/getinfo  文档在用户接口-群组信息管理-查询群组信息下
- [x] 首页接口文档已更新，所有的产品列表新增 imageUrl 【背景图】字段
- [x] 【产品列表】 /api/product/list 返回json结构变化
- [x] 【产品列表】新增接口：/api/product/list/{productType}   【看情况使用，/api/product/list 已返回所有数据，tab滑动可以在前端做筛选】
- [x] 【产品列表】展示规则，根据 数量 和 列表顺序展示， 非三个的情况下用宽版，等于三个的情况下用方块,后端图片已适配
- [x] 【config接口】 新增 产品分类的 tab的配置
- [x] 【产品详情】新增 优惠券赠送 、 返佣比例、介绍、详情图
- [x] 【产品详情-可用优惠券】 新增结束日期字段
- [x] 【购买列表】接口新增payStatus参数，过滤付款状态 /api/product/order/pageList/{payStatus}  接口新增字段imgUrl3(底图3url，横图)、holdStartTime（购买日期）
- [x] 【我的优惠券】接口 删除开始日期字段
- [x] 【岗位列表】接口 /api/post/postlist 奖励发放周期为config参数中key值为profit_cycle的数据；具体值为 {"profitCycleName": "周", "profitTime":"5"}// 每周五晚上八点开始发放（晚上八点定死的）

![image](https://user-images.githubusercontent.com/37478475/177053247-7b1df513-c2e0-42aa-92a3-03f50071c491.png)

## 未完成接口



- [ ] 7、 推广页面 隐藏产品 【每日收益】 的返佣 
- [x] 8、 新增 【岗位】列表查询接口,图标由前端按顺序展示，后端最多返回五个岗位，
- [ ] 岗位列表下面显示 岗位津贴发放时间：每周五八点发放津贴，config接口新增此字符串
- [ ] 岗位列表下面显示 中国能源集团每周会为有贡献的成员发放岗位津贴，联系客服了解详细情况，跳转到客服页，UI待设计
- [ ] 9、 【产品日志】 新增收益字段
- [x] 【持有】接口 返回格式按 日期list-产品list嵌套
- [x] 关于我们新增 【官方群聊】 接口
- [ ] 持有日志新增金额字段

![image](https://user-images.githubusercontent.com/106216124/177014681-09aa9e87-dfaf-4b92-b2e4-019935999944.png)


## 前端单独修改
- [ ] 提现接口固定传人民币的参数，且不需要查询汇率
- [ ] 本系统只有人民币一种，提现是人民币usdt的选项改为 提现至 卡号，跟上个


## 后端单独修改
- [ ] 优化聊天组件
- [ ] 取消状态修改功能
- [√] 取消每日收益返佣
- [ ] 注册赠送优惠券【默认Lv1赠送】
- [ ] 产品锁定周期 为 永久锁定，不可卖出

![image](https://user-images.githubusercontent.com/106216124/176252621-2edcf538-1618-47fb-9841-069bf9697c22.png)

