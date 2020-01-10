# PRD_Museum

|   Title  |   Content  |
| --- | --- |
|  Date(发布日期)  |  2019/12  |
|   Epic(史诗名称) |   动静相宜博物馆  |
|    Document status(文档状态) |  进行中   |
|  Document owner(文件主人)  |  莫熙彤  |
|  Designer(领头的设计师)  |  莫熙彤  |
|  Developer(领头的开发者)  |   莫熙彤  |
|  QA(领头的测试者)  |  莫熙彤  |

## 产品文档目录
[PRD价值主张设计](#PRD价值主张设计)
- [PRD1.加值宣言](#PRD1加值宣言)
- [PRD2.核心价值](#PRD2核心价值)
- [PRD3.核心价值与用户痛点](#PRD3核心价值与用户痛点)
- [PRD4.人工智能概率性与用户痛点](#PRD4人工智能概率性与用户痛点)
- [PRD5.需求列表与人工智能API加值](#PRD5需求列表与人工智能API加值)

[原型20%](#原型20%)
- [原型1.交互及界面设计](#原型1交互及界面设计)
- [原型2.信息设计](#原型2信息设计)
- [原型3.原型文档](#原型3原型文档)

[API 产品使用关键AI或机器学习之API的输出入展示 15%](#API产品使用关键AI或机器学习之API的输出入展示)
- [API1.使用水平](#API1使用水平)
- [API2.使用比较分析](#API2使用比较分析)
- [API3.使用后风险报告](#API3使用后风险报告)
- [API4.加分项](#API4加分项)

## PRD价值主张设计

### PRD1加值宣言

- 一句话版本：动静相宜博物馆，地图规划无困难；再加上语音合成，一切变得好简单；危险行为识别在，跌倒也会有人爱

- 一分钟版本：市面上许多身体残障人士因为身体部分功能的缺失以及不受控制等的原因无法在博物馆中享受到与正常人一样欣赏展览品的能力，他们需要一款产品来帮助他们游览博物馆，设定更适合他们的博物馆路径规划图；通过语音合成服务帮助他们更好地理解展览品的文化价值；以及时刻监测他们游览时的状态

- 目标用户：
身体障碍者、多动症患者等其他身体不够健全的人群、年级较小的用户以及老年人

### PRD2核心价值

1.根据每位使用者的特点在博物馆内设定路线规划图

2.用户能选择喜欢的软件人声去合成展览品的相关信息朗读

3.通过与博物馆授权的摄像头监测到危险行为，当此类用户出现失控状态下及时发出警报通知身边人帮忙

### PRD3核心价值与用户痛点

1.身障者以及多动症患者通常不善于与人交流

2.他们对于同一件展览品所播放的相关信息可能需要更细致的讲解

3.在遇到困难时无法及时地得到帮助

4.他们通常对于博物馆印制的普通地图不太看得懂

### PRD4人工智能概率性与用户痛点

- 室内地图API（高德开放平台）

此产品可以令开发者可以轻松地开发出室内地图显示与操作、兴趣点搜索、室内路线规划等功能，但高德未覆盖的室内地图数据，需要委托高德室内数据生产认证合作商生产，并不能确保每家博物馆都为高德提供了数据。

- 语音合成API（阿里云）

此产品在技术上兼顾了多级韵律停顿，达到自然的合成韵律目的，综合利用声学参数和语言学参数，建立基于深度学习的多重自动预测模型；使用海量的音频数据训练合成数据，合成音真实饱满、抑扬顿挫、富有表现力，MOS评分达到业内顶级水准。此产品提供了多种语音供用户选择，满足了用户的多样性设置，但不同语音的朗读顺畅度不同，可能部分会出现卡顿的词语。

- 危险行为识别API（百度云）

此产品目前支持单人、双人场景，更多场景和行为还在持续扩展中，这意味着如果用户在人流量较多的区域发生了疾病等突发情况不能及时进行察觉。

### PRD5需求列表与人工智能API加值

#### 需求列表

|   用户需求  |   对应标题  |  重要程度  |
| ----- | ----- | ----- |
|   在手机上得到博物馆内的路线规划图 |   路线  |  重要  |
|   展览品的相关信息朗读 |  展品集   |  重要  |
|  需求帮助警报提示  |  系统主动发出  |  次重要  |

#### 人工智能API加值

- 室内地图API（高德开放平台）

高德室内地图提供最优质专业的室内地图及定位服务，帮客户解决难题

- 语音合成API（阿里云）

语音合成服务，通过先进的深度学习技术，将文本转换成自然流畅的语音。目前有多种音色可供选择，并提供调节语速、语调、音量等功能。适用于智能客服、语音交互、文学有声阅读和无障碍播报等场景。

- 危险行为识别API（百度云）

针对5S内的监控视频片段，识别常见危险行为，如摔倒、砸东西、拉扯、推搡、踢踹等，实时监控分析人员行为，及时发现人摔倒等危险情况，保障人身安全

## 原型
### 原型1交互及界面设计

- 首页

![首页](https://gitee.com/NFUNM066/API/raw/master/%E9%A6%96%E9%A1%B5.png)

1.首页显示有关博物馆的信息滚动页面，并设置了推荐页面，可供用户进行搜索

2.底部菜单栏图标均可实现点击跳转至相应页面的效果

- 地图

![地图](https://gitee.com/NFUNM066/API/raw/master/%E5%9C%B0%E5%9B%BE.png)

1.用户先在此处选择喜欢的展品风格、偏好的游览路线，然后再点击选择完毕将生成地图

2.底部菜单栏图标均可实现点击跳转至相应页面的效果。

- 生成地图

![生成地图](https://gitee.com/NFUNM066/API/raw/master/%E7%94%9F%E6%88%90%E5%9C%B0%E5%9B%BE.png)

1.这里显示系统生成的地图，用户如果不满意可以进行重新设置，返回到设置页面

2.底部菜单栏图标均可实现点击跳转至相应页面的效果。

- 我

![我](https://gitee.com/NFUNM066/API/raw/master/%E6%88%91.png)

1.身体残障者用户可以在“我的秘密”设置自己的身体情况，系统将根据情况推荐路线

2.“系统警报”按钮将在用户出现身体情况时自动响起

3.“我”页面设置了消息通知、浏览历史等页面、供人们进行查看

4.底部菜单栏图标均可实现点击跳转至相应页面的效果

### 原型2信息设计

![产品架构图](https://gitee.com/NFUNM066/API/raw/master/%E4%BA%A7%E5%93%81%E6%9E%B6%E6%9E%84.jpg)

### 原型3原型文档

- [动静相宜博物馆-原型文档](http://nfunm066.gitee.io/api/#id=rfh50x&p=%E9%A6%96%E9%A1%B5&g=1)
- [动静相宜博物馆-原型文档下载](https://gitee.com/NFUNM066/API)

## API产品使用关键AI或机器学习之API的输出入展示
### API1使用水平

1.根据用户的特性进行路线规划（路线规划API 高德开放平台）

- 调用状态：

![室内地图](https://gitee.com/NFUNM066/first/raw/master/%E5%AE%A4%E5%86%85%E5%9C%B0%E5%9B%BE.png)

```


//当前界面的mapView
@property (nonatomic, strong) BMKMapView *mapView; 

- (void)viewDidLoad {
    [super viewDidLoad];
    _mapView = [[BMKMapView alloc] initWithFrame:self.view.bounds];
    //设置mapView的代理
    _mapView.delegate = self;
    //将mapView添加到当前视图中
    [self.view addSubview:_mapView];
}

- (void)viewWillAppear:(BOOL)animated {
    [super viewWillAppear: animated];
    //当mapView即将被显示的时候调用，恢复之前存储的mapView状态
    [_mapView viewWillAppear];
}

- (void)viewWillDisappear:(BOOL)animated {
    [super viewWillDisappear: animated];
    //当mapView即将被隐藏的时候调用，存储当前mapView的状态
    [_mapView viewWillDisappear];
}
                      

```

2.展览品的相关信息朗读（语音合成API 阿里云）

- 输入：展览品信息、喜欢的声音

![清明上河图](https://gitee.com/NFUNM066/first/raw/master/%E6%B8%85%E6%98%8E%E4%B8%8A%E6%B2%B3%E5%9B%BE.png)

- 输出：语音朗读文件

![语音合成](https://gitee.com/NFUNM066/first/raw/master/%E8%AF%AD%E9%9F%B3%E5%90%88%E6%88%90.png)

3.需求帮助警报提示（危险行为识别API 百度云）

- 输入：监控录像片段

![摔倒](https://gitee.com/NFUNM066/first/raw/master/%E6%91%94%E5%80%92.jpg)

- 输出：单人场景，识别4类常见危险行为，包括：情绪性指人、摔倒、激烈抱怨、砸东西。

### API2使用比较分析

#### 1.室内规划

- [高德-室内地图](https://lbs.amap.com/api/javascript-api/reference/indoormap)
- [蜂鸟云-室内地图](https://www.fengmap.com/)

|   对比项  |   高德云  |  蜂鸟云  |
| ----- | ----- | ----- |
|   成熟度 |   文档清晰且详细，旗下的API比较细分，能满足多方面的需要   |   文档较为完善，但涉及到的功能过少，并且知名度不高 |
|   性价比 |  180元/月-300元/月  |  150元/月-300元/月  |

#### 2.语音合成技术

- [阿里云-语音技术-语音合成](https://help.aliyun.com/document_detail/84881.html?spm=5176.12061040.1251723..3bff47790bLkNC)
- [百度云-语音技术-语音合成](https://ai.baidu.com/ai-doc/SPEECH/Gk38y8lzk)

|   对比项  |   阿里云  |  百度云  | 
| ----- | ----- | ----- | 
|   成熟度 |   文档清晰且详细，旗下的API比较细分，能满足多方面的需要；价格优惠   |   产品文档清晰明了 | 
|   性价比（以驾驶证识别为例） |  1.1元/千次-1.8元/千次  |  5元/个~商务沟通  |

### API3使用后风险报告

#### API市场竞争程度

1.室内地图API（高德开放平台）

- 从搜索结果看，高德在baidu上的搜索结果为第一名，可以推测高德的室内地图使用面积还是较广的。
- 从竞争对手看，目前市面上拥有室内地图api技术的公司数量较少，高德可以继续建立自身的产品优势以及价格优势来站稳脚跟

2.语音合成API（阿里云）

- 从使用感受和快捷度来看，阿里云此款api还是比较成熟的，还有一个免费使用的平台供潜在用户进行测试使用，可以满足用户“货比三家”的需求。

#### 输入输出限制

1.室内规划API（高德）

- 输入：gps定位
- 输出：地图信息

2.语音合成API（阿里云）

- 输入：文本内容
- 输出：所合成的音频文件

#### 定价

1.室内规划API（高德开放平台）

- 180元/月-300元/月

2.语音合成API（阿里云）

- 1.1元/小时-1.8元/小时

### API4加分项

使用复杂度：已使用2个人工智能API之输入输出，分别是[室内地图API](https://lbs.amap.com/getting-started/indoorintro)、[语音合成API](https://ai.baidu.com/tech/speech/tts?track=cp:ainsem|pf:pc|pp:chanpin-yuyin|pu:yuyin-yuyinhecheng-pinpai|ci:|kw:10003541)、[危险行为识别](https://cloud.baidu.com/product/body/danger)
