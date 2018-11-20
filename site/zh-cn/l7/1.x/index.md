<!--
template: home
title: L7
keywords:
  - L7
  - 地理
  - 空间可视化
  - Webgl
  - 地图
  - 3d
  - GIS Mapbox deckgl
description: L7 中的 L 代表 Location，7 代表世界七大洲，寓意能为全球位置数据提供可视化能力。L7 的目标是提供一套地理空间数据可视化框架，易用易扩展，支持海量数据的高性能和 3D 高质量渲染，安全可靠（无地图法务风险）的地理空间数据可视化解决方案。
featuresCards:
  - img: ${assets}/image/home/features-professional.svg
    title: 架构上灵活可扩展
    description: 围绕设计、性能以及异构环境，为用户提供移动端图表的最佳实践
  - img: ${assets}/image/home/features-simple.svg
    title: 业务上简洁、通用
    description: 基于图形语法，可灵活构建各类图表（50+），组件完备，覆盖各类场景
  - img: ${assets}/image/home/features-powerful.svg
    title: 可视化上酷炫，动感
    description: 插件机制，图形、动画、交互均可灵活扩展，使用更自由
usecases:
  - img: ${assets}/image/home/f2/usecase-caifu.png
    icon: ${assets}/image/home/f2/caifu-logo.png
    title: 蚂蚁财富
    description: 已广泛应用于基金、定期、黄金、股票等各个金融业务场景中，支撑着蚂蚁财富 app 上众多可视化场景。同时通过深入剖析用户的可视化诉求，沉淀出多套面向金融的可视化方案。
    relate: true
    name: 基金可视化设计方案
    link: https://www.yuque.com/mo-college/f2-fund-course
  - img: ${assets}/image/home/f2/usecase-alipay.png
    icon: ${assets}/image/home/f2/alipay-logo.png
    title: 支付宝
    description: 覆盖蚂蚁会员、支付宝月账单、个人总资产等业务场景，通过可视化的形式帮助您更快更好得了解您的消费数据。
  - img: ${assets}/image/home/f2/usecase-tpp.png
    icon: ${assets}/image/home/f2/tpp-logo.png
    title: 淘票票专业版
    description: 助力票房数据、受众画像、播放量等可视分析场景，帮助用户更好地洞察数据背后的信息以做出更好的决策。
clients:
  - img: ${assets}/image/home/f2/mayicaifu.png
  - img: ${assets}/image/home/f2/taopiaopiao.png
  - img: ${assets}/image/home/f2/dingding.png
  - img: ${assets}/image/home/f2/zhangshangyunwei.png
  - img: ${assets}/image/home/f2/alipay.png
  - img: ${assets}/image/home/f2/xiaohongshu.png
  - img: ${assets}/image/home/f2/hema.png
  - img: ${assets}/image/home/f2/koubei.png
resource:
  jsFiles:
    - ${url['f2-all']}
-->

<!-- 第一屏，产品简介 -->
<section class="intro">
  <div class="container">
    <div class="header row">
      <div class="col-md-5">
        <h1> L7 地理空间数据可视化</h1>
        <p class="main-info">L7 中的 L 代表 Location，7 代表世界七大洲，寓意能为全球位置数据提供可视化能力。L7 的目标是提供一套地理空间数据可视化框架，易用易扩展，支持海量数据的高性能和 3D 高质量渲染，安全可靠（无地图法务风险）的地理空间数据可视化解决方案。</p>
        <a href="{{ products.f2.getStarted.href }}" class="btn btn-primary btn-lg btn-round-link">{{ products.f2.getStarted.text }}</a>
        <iframe class="btn-round-link btn btn-light btn-lg github-btn" src="https://ghbtns.com/github-btn.html?user=antvis&repo=f2&type=star&count=true&size=large" frameborder="0" scrolling="0" width="170px" height="20px"></iframe>
      </div>
      <div class="col-md-7">
        <div class="demo-container">
        <div class="f2-chart-wrapper">
          <div class="chart-header">
          <div id="chartTitle">商品价格 7 年走势对比</div>
          </div>
          <div class="chart-content">
          <div class="contianer slick">
            <div id="commentsCarousel" class="carousel">
            <div class="carousel-inner slick">
              <div class="carousel-item active">
              <canvas id="c1"></canvas>
              </div>
              <div class="carousel-item">
              <canvas id="c2"></canvas>
              </div>
              <div class="carousel-item">
              <canvas id="c3"></canvas>
              </div>
            </div>
            </div>
          </div>
          </div>
        </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- 第二屏：产品特性 -->
<section class="features text-center">
  <div class="container">
    <div class="row">
    {% for card in featuresCards %}
      <div class="feature col-md-4 text-center">
        <img src="{{ card.img }}" alt="" width="120" height="120">
        <h5>{{ card.title }}</h5>
        <div class="detail">{{ card.description }}</div>
      </div>
    {% endfor %}
    </div>
  </div>
</section>

<!-- 第三屏：使用案例 -->
<section class="use-cases">
  <div class="container slider">
    {% for card in usecases %}
    <div class="row test">
      <div class="col-md-7">
        <img class="case-image" src="{{ card.img }}" />
      </div>
      <div class="col-md-5 case-content">
        <div class="logo">
          <img src="{{ card.icon }}" />
        </div>
        <div class="title">{{ card.title }}</div>
        <div class="description">{{ card.description }}</div>
        {% if card.relate %}
        <div class="relate">
          <div class="flex">
            <div class="item name">{{ card.name }}</div>
            <div class="item link">
              <a href="{{ card.link }}" target="_blank">查看详情></a>
            </div>
          </div>
        </div>
        {% endif %}
      </div>
    </div>
    {% endfor %}
  </div>
</section>

<!-- 第四屏 使用 app -->
<section class="clients-container">
  <div class="container">
    <div class="title text-center">感谢一路合作的伙伴</div>
    <div class="row">
      {% for card in clients %}
      <div class="col-md-3">
        <img class="client-icon" src="{{ card.img }}" />
      </div>
      {% endfor %}
    </div>
  </div>
</section>

<!-- F2 二维码展示容器 -->
<div style="position: absolute;">
  <div class="scancode-wrapper">
    <div class="scancode-content">
      <div class="scancode-arrow"></div>
      <div class="scancode-inner">
        <div id="scanCode" data-url={{ products.f2.qrCode.href }} ></div>
      </div>
    </div>
  </div>
</div>


```js-
// F2 第一屏的图表滚动代码
var names = ['商品价格 7 年走势对比', '层叠条形图', '饼图'];

$('.chart-content .slick').each(function () {
  var $target = $(this);
  $target.slick({
    slidesToShow: 1,
    adaptiveHeight: true,
    infinite: true,
    speed: 500,
    cssEase: 'linear',
    arrows: false,
    autoplay: true,
    autoplaySpeed: 2000,
    fade: true,
  }).on('beforeChange', function (event, slick, currentSlide, nextSlide) {
    $('#chartTitle').text(names[nextSlide]);
  });
});
```

<!-- chart1 折线图 -->
```js-
  $.getJSON('/assets/data/f2/series-line.json', function(data) {
    var chart = new F2.Chart({
      id: 'c1',
      pixelRatio: window.devicePixelRatio
    });
    chart.source(data);
    chart.scale('date', {
      type: 'timeCat',
      tickCount: 3
    });
    chart.scale('value', {
      tickCount: 5
    });
    chart.axis('date', {
      label: function(text, index, total) {
        // 只显示每一年的第一天
        var textCfg = {};
        if (index === 0) {
          textCfg.textAlign = 'left';
        }
        if (index === total - 1) {
          textCfg.textAlign = 'right';
        }
        return textCfg;
      }
    });
    chart.tooltip({
      custom: function(obj) {
        var legend = chart.get('legendController').legends.top[0];
        var tooltipItems = obj.items;
        var legendItems = legend.items;
        var map = {};
        legendItems.map(function(item) {
          map[item.name] = _.clone(item);
        });
        tooltipItems.map(function(item) {
          var name = item.name;
          var value = item.value;
          if (map[name]) {
            map[name].value = value;
          }
        });
        legend.setItems(_.values(map));
      },
      onHide: function() {
        var legend = chart.get('legendController').legends.top[0];
        legend.setItems(chart.getLegendItems().country);
      }
    });
    chart.line().position('date*value').color('type');
    chart.render();
  });
```

<!-- chart2 层叠条形图 -->
```js-
  var data = [
    { State: 'WY', 年龄段 : '小于5岁', 人口数量: 25635 },
    { State: 'WY', 年龄段 : '5至13岁', 人口数量: 1890 },
    { State: 'WY', 年龄段 : '14至17岁', 人口数量: 9314 },
    { State: 'DC', 年龄段 : '小于5岁', 人口数量: 30352 },
    { State: 'DC', 年龄段 : '5至13岁', 人口数量: 20439 },
    { State: 'DC', 年龄段 : '14至17岁', 人口数量: 10225 },
    { State: 'VT', 年龄段 : '小于5岁', 人口数量: 38253 },
    { State: 'VT', 年龄段 : '5至13岁', 人口数量: 42538 },
    { State: 'VT', 年龄段 : '14至17岁', 人口数量: 15757 },
    { State: 'ND', 年龄段 : '小于5岁', 人口数量: 51896 },
    { State: 'ND', 年龄段 : '5至13岁', 人口数量: 67358 },
    { State: 'ND', 年龄段 : '14至17岁', 人口数量: 18794 },
    { State: 'AK', 年龄段 : '小于5岁', 人口数量: 72083 },
    { State: 'AK', 年龄段 : '5至13岁', 人口数量: 85640 },
    { State: 'AK', 年龄段 : '14至17岁', 人口数量: 22153 }
  ];
  var chart = new F2.Chart({
    id: 'c2',
    pixelRatio: window.devicePixelRatio
  });

  chart.source(data, {
    '人口数量': {
      tickCount: 5
    }
  });
  chart.coord({
    transposed: true
  });
  chart.axis('State', {
    line: F2.Global._defaultAxis.line,
    grid: null
  });
  chart.axis('人口数量', {
    line: null,
    grid: F2.Global._defaultAxis.grid,
    label: function(text, index, total) {
      var textCfg = {
        text: text / 1000 + ' k'
      };
      if (index === 0) {
        textCfg.textAlign = 'left';
      }
      if (index === total - 1) {
        textCfg.textAlign = 'right';
      }
      return textCfg;
    }
  });
  chart.tooltip({
    custom: function(obj) {
      var legend = chart.get('legendController').legends.top[0];
      var tooltipItems = obj.items;
      var legendItems = legend.items;
      var map = {};
      legendItems.map(function(item) {
        map[item.name] = _.clone(item);
      });
      tooltipItems.map(function(item) {
        var name = item.name;
        var value = item.value;
        if (map[name]) {
          map[name].value = (value);
        }
      });
      legend.setItems(_.values(map));
    },
    onHide: function() {
      var legend = chart.get('legendController').legends.top[0];
      legend.setItems(chart.getLegendItems().country);
    }
  });
  chart.interval().position('State*人口数量').color('年龄段').adjust('stack');

  chart.render();
```

<!-- chart3 带文本的饼图 -->
```js-
const data = [
    { const: 'const', type: '交通出行', money: 51.39 },
    { const: 'const', type: '饮食', money: 356.68 },
    { const: 'const', type: '生活日用', money: 20.00 },
    { const: 'const', type: '住房缴费', money: 116.53 }
  ];
  const chart = new F2.Chart({
    id: 'c3',
    padding: 0,
    appendPadding: 0,
    pixelRatio: window.devicePixelRatio
  });
  chart.source(data);
  chart.coord('polar', {
    transposed: true,
    radius: 0.5,
    innerRadius: 0.5
  });
  chart.axis(false);
  chart.legend(false);
  chart.tooltip(false);
  chart.guide().html({
    position: [ '50%', '50%' ],
    html: `<div style="text-align: center;width:150px;height: 50px;">
      <p style="font-size: 12px;color: #999;margin: 0" id="title"></p>
      <p style="font-size: 18px;color: #343434;margin: 0;font-weight: bold;" id="money"></p>
      </div>`
  });
  chart.interval()
    .position('const*money')
    .adjust('stack')
    .color('type', ['#1890FF', '#13C2C2', '#2FC25B', '#FACC14']);
  chart.pieLabel({
    sidePadding: 8,
    activeShape: true,
    label1(data) {
      return {
        text: '￥' + data.money,
        fill: '#343434',
        fontWeight: 'bold'
      };
    },
    label2(data) {
      return {
        text: data.type,
        fill: '#999'
      };
    },
    onClick(ev) {
      const data = ev.data;
      if (data) {
        $('#title').text(data.type);
        $('#money').text(data.money);
      }
    }
  });
  chart.render();
```