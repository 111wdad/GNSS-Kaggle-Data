# GNSS-Kaggle-Data
## gnss_comparsion_results

数据包含wls_estimate.csv与groundtuth.csv数据的平均偏差(米),最大偏差(米),最小偏差(米),标准差(米),中位数偏差(米),95%偏差(米)



## continuous_error_segment-[error_threshold]

从样本数据中抽样出大偏差数据点

抽样原则：连续的100个偏差大于error_threshold的点作为一个数据块

### 数据格式理解

在continuous_error_segments.csv中：

`lat_rx_wls_deg, lon_rx_wls_deg, alt_rx_wls_m` 是WLS估计值（程序计算值）

`latDeg, lngDeg, heightAboveWgs84EllipsoidM` 是对应的真实值（ground truth）

`distance_error` 是两者之间的偏差（米）

`timestamp` 是时间戳

`folder` 是数据来源文件夹

