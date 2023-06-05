# gcn_colab
利用硬件实现矩阵乘法加速
參考：
学过计算机组成原理的都知道，CPU访问内存的速度比CPU计算速度慢得多，为了解决速度不匹配的问题，在CPU与内存之间加了高速缓存cache。cache的存在大大提高了CPU访问数据的速度。由于价格等原因，cache都比较小。因此，较好地利用cache可以加速程序运行。


case比較：
矩陣鏈乘法（或矩陣鏈排序問題[1]）是關於以最有效的方式乘以給定矩陣序列的優化問題。問題實際上不是執行乘法，而只是決定所涉及的矩陣乘法的順序。該問題可以使用動態規劃來解決。


新增cuda混合編譯

參考：
https://blog.csdn.net/zzc_zhuyu/article/details/89929129
https://github.com/hengdashi/cuda_gcn/tree/main
https://blog.csdn.net/weixin_56273009/article/details/127449183?utm_medium=distribute.pc_relevant.none-task-blog-2~default~baidujs_baidulandingword~default-4-127449183-blog-89929129.235^v36^pc_relevant_default_base&spm=1001.2101.3001.4242.3&utm_relevant_index=5
https://en.wikipedia.org/wiki/Matrix_chain_multiplication
