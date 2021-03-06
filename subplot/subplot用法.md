<h1><center>subplot用法</center></h1>

# 基本用途

* 一張Figure若想要含有多張子圖,就可以使用subplot這個函數來繪製

# 基本語法

* 其語法的構成為subplot(number_row,number_column, plot_number)
  * number_row為圖總共有幾列
  * number_column為圖總共有幾行
  * plot_number為指第幾個圖

# 基礎例子

* 範例1:

![1](https://github.com/bruce-dmlab/Matplotlib/blob/master/subplot/123.png?raw=true)

​				上述的程式碼,其運作會將一張圖切成2列2行共四等份,如果要說明清楚一些,大		概就像下圖：

![1](https://github.com/bruce-dmlab/Matplotlib/blob/master/subplot/234.png?raw=true)

​				上圖整個表格就像一張圖,而欄就相當於一張子圖,其中欄裡的編號則代表為第幾		張子圖

# 進階例子

* 範例2:

![1](https://github.com/bruce-dmlab/Matplotlib/blob/master/subplot/345.png?raw=true)

​				上述的程式碼會複雜一些,從程式碼中可以看到我們總共要畫上4張子圖,接著讓		我們分成六個步驟來抽絲剝繭,看看這段程式要說些什麼：	

   1. 首先會先建立一張圖,如下圖

      ![1](https://github.com/bruce-dmlab/Matplotlib/blob/master/subplot/456.png?raw=true)

      可以看到目前圖上沒有任何的子圖,也沒有在圖上畫上任何東西

			2. 接著我們將圖以2*2的方式進行劃分,並在編號1的位置做圖

      ![1](https://github.com/bruce-dmlab/Matplotlib/blob/master/subplot/567.png?raw=true)

      此時能看到在2*2之中,編號1的位置被做圖了

			3. 接著我們將整張圖以6*4重新劃分

      ![1](https://github.com/bruce-dmlab/Matplotlib/blob/master/subplot/678.png?raw=true)

      其中米黃色的部份為第一張子圖佔據的部份,淺藍色的部份為第二張子圖所佔據的部份

			4. 接著第三張子圖將佔用編號13的位置做圖

      ![1](https://github.com/bruce-dmlab/Matplotlib/blob/master/subplot/789.png?raw=true)

			5. 將圖再以2*2重新劃分,並在2 * 2中編號4的位置作圖,此時2 * 2 與 4 * 4編號的對應關係如下圖

      ![1](https://github.com/bruce-dmlab/Matplotlib/blob/master/subplot/8910.png?raw=true)

      2 * 2 與 6 * 6的編號對應如下

      * 1 -> 1 2 5 6 9 10
      * 2 -> 3 4 7 8 11 12
      * 3 -> 13 14 17 18 21 22
      * 4 -> 15 16 19 20 23 24

      其中粉紅色的部份為第四張子圖所佔據的編號

			6.  最後來看看程式碼執行結果八

      ![1](https://github.com/bruce-dmlab/Matplotlib/blob/master/subplot/91011.png?raw=true)