# 驱动数据下载与处理


## GLDASV21
<https://disc.gsfc.nasa.gov/datasets/GLDAS_NOAH025_3H_2.1/summary>

`aria2c`下载，`cdo`拼接。

```bash
# 换用自己的账户和密码
aria2c -c -x4 -j4 -i subset_GLDAS_NOAH025_3H_2.1_20220419_015925.txt -d GLDASV2.1 --http-user JaneKong --http-passwd passwd
```

## ERA5-Land
采用GEE下载daily的数据（小区域）
