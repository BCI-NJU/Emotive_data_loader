### 数据类型
1. _orginal.npy：原始数据没有滤波后的数据，数据结构为二维数组，每一行的数据，为某个时刻下的各个数据

        ["COUNTER","INTERPOLATED", "AF3","F7","F3","FC5","T7","P7","O1","O2","P8","T8","FC6","F4","F8","AF4", "RAW_CQ", "MARKER_HARDWARE", "time"]
2. _processed.npy：滤波后的数据，数据为二维，一共是（15,"time"）最后一行为时间, 前14行分别为
   
        [ "AF3","F7","F3","FC5","T7","P7","O1","O2","P8","T8","FC6","F4","F8","AF4"]


### 数据处理
+ data_processing中有data_processing函数，传入原始数据，和所需处理阶数，即可得到最终结果，本data中的处理后数据为默认2阶处理

        ex: left_hand_processed = data_processing(lef_hand_orgianl, 2)