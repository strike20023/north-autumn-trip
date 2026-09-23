# 苹果地图地点链接

网站使用本机 macOS MapKit 的 MKLocalSearch 返回地点ID，核对名称、地址和既有位置后，生成 /place?place-id= 链接。没有使用关键词拼接，不把商家官网字段当成地图链接。

正式景区入口、售票处与园内景点有区别。匹配不确定的地点不显示苹果链接。地图线路仍采用原有高德道路数据。

本机原生查询成功；当前内置浏览器中 Apple 地图中国网页返回了非预期HTML，导致地点面板加载失败。网页打开和 iPhone 唤端尚不能标为全部验证通过。可使用高德入口；苹果设备可尝试在 Safari 中打开。

官方文档：
- https://developer.apple.com/documentation/mapkit/unified-map-urls
- https://developer.apple.com/documentation/mapkit/mklocalsearch/request
- https://developer.apple.com/maps/place-id-lookup/

具体地点与匹配记录见 apple-map-places.json。
