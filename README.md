# lyh-Dataset

> [!Note]
> If you would like to use this dataset, we assume that you've **agreed with us on the following statements**:
> - **No Commercial Use**: The user may only use the dataset for academic research.
> - **No Warranty**: The dataset comes without any warranty, the BCI-VR group cannot be held accountable for any damage(physical, financial, or otherwise) caused by the use of the dataset.

## Acquisition of the dataset


<details closed>
  <summary>Chinese Version of Explanation</summary>

**orginal数据**

_orginal数据为未滤波的数据

形式为(n,), n是4s采样的次数，目前为300次

第一个维度为4s实验次数

下一个维度为4s中采集的数据的个数，因为为250hz，所以是1000个数据左右，但是有波动

下一个维度为单个采样数据，长度19，分别为：["COUNTER","INTERPOLATED", "AF3","F7","F3","FC5","T7","P7","O1","O2","P8","T8","FC6","F4","F8","AF4", "RAW_CQ", "MARKER_HARDWARE"， "time"]

**processed数据**

_processed为滤波后数据

形式为(15, m)m为总采样点数，m = n4250, 目前为300000

15分别为["AF3","F7","F3","FC5","T7","P7","O1","O2","P8","T8","FC6","F4","F8","AF4", "time"]

</details>



