# gcn_colab
利用硬件实现矩阵乘法加速
參考：
学过计算机组成原理的都知道，CPU访问内存的速度比CPU计算速度慢得多，为了解决速度不匹配的问题，在CPU与内存之间加了高速缓存cache。cache的存在大大提高了CPU访问数据的速度。由于价格等原因，cache都比较小。因此，较好地利用cache可以加速程序运行。
case比較：
斯特拉森算法把原先普通二階矩陣相乘需要的8次乘法壓縮到7次乘法，而在計算機，乘法運算的耗時遠遠高於加減運算，所以斯特拉森算法可以將O(d^ 3) 壓縮到O(d^2.8)。需要知道的是，斯特拉森算法只是對矩陣分治的算法而不是單獨的乘法算法，分治完成時最後使用的還是普通矩陣乘法，在階數小於等於32（或者64？看過不同的實驗結果）時普通的矩陣乘法會有更快的速度，而隨著矩陣的階不斷增加，斯特拉森可以提供更快的速度。


新增cuda混合編譯

參考：
https://blog.csdn.net/zzc_zhuyu/article/details/89929129
https://github.com/hengdashi/cuda_gcn/tree/main
https://blog.csdn.net/weixin_56273009/article/details/127449183?utm_medium=distribute.pc_relevant.none-task-blog-2~default~baidujs_baidulandingword~default-4-127449183-blog-89929129.235^v36^pc_relevant_default_base&spm=1001.2101.3001.4242.3&utm_relevant_index=5
