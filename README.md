# 2020 Tawainese-general-election
----
## Description
> 透過政府開放式資料:  
> 1.2020總統(副總統)選舉資料(xls)  
> 2.2020不分區立委選舉資料(xls)  
> 3.台灣地理資訊(shp)  
> 繪製台灣總統得票率藍綠版圖、不分區立委得票率與藍綠總統候選人得票率關係圖
----
## Process&Insight
1. 用正規表示式匯入所需投票資訊檔案   
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E6%AD%A3%E8%A6%8F%E8%A1%A8%E7%A4%BA%E5%BC%8F%E8%AE%80%E5%8F%96%E4%BE%86%E6%BA%90%E8%B3%87%E6%96%99.PNG)
2. 透過Function清理投票資訊  
> (1)整理前
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E7%B8%BD%E7%B5%B1%E5%BE%97%E7%A5%A8%E7%8E%87%E5%8E%9F%E5%A7%8B%E8%B3%87%E6%96%99.PNG)
> (2)整理後  
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E7%B8%BD%E7%B5%B1%E5%BE%97%E7%A5%A8%E7%8E%87%E8%BD%89%E6%8F%9B%E5%BE%8C.PNG)
3. 匯入shp檔，整理地理資訊  
> (1)整理前  
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E5%9C%B0%E7%90%86%E5%8E%9F%E5%A7%8B%E8%B3%87%E6%96%99.PNG)  
> (2)整理後  
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E5%9C%B0%E7%90%86%E8%B3%87%E6%96%99%E8%BD%89%E6%8F%9B%E5%BE%8C.PNG)  
4. 資料縣市與鄉鎮市區得票率視覺化  
> :bulb:KPI為蔡英文得票率，由高到低顏色對應為綠->白->藍  
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E7%B8%BD%E7%B5%B1%E5%BE%97%E7%A5%A8%E7%8E%87%E8%97%8D%E7%B6%A0%E7%89%88%E5%9C%96.PNG)  
> :bulb:以縣市來看的話，可以發現嘉義縣與屏東縣是非常綠的；金門縣與連江縣是非常藍的。  
> :bulb:以鄉鎮市區來看的話，可以發現南投、花蓮、台東其實部分鄉鎮市區很藍，但也有部分鄉鎮市區相較不藍，所以若以縣市角度來看整體較金門縣與連江縣不藍  
5. 高票地區與藍綠候選人差距小選區  
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E8%A1%A8%E6%A0%BC%E5%88%86%E6%9E%90.PNG)  
6. 加入不分區立委資料(資料匯入與清理同1&2)，透過散佈圖分析鄉鎮市區的19個不分區政黨得票率與兩總統候選人得票率關係  
> :bulb:若散佈圖與紅線重疊(斜率=1)，表示支持該政黨的鄉鎮市區也支持該黨總統候選人  
> (1)各政黨與蔡英文
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E6%94%BF%E9%BB%A8%E5%BE%97%E7%A5%A8%E7%8E%87%E8%88%87%E8%94%A1%E5%BE%97%E7%A5%A8%E7%8E%87%E9%97%9C%E4%BF%82%E5%9C%96.PNG)  
> :bulb:民主進步黨與蔡英文得票率高度正相關，斜率>1，蔡英文票源主要為民主進步黨，並非完全民主進步黨  
> :bulb:中國國民黨與蔡英文得票率高度負相關  
> :bulb:民主進步黨與蔡英文得票率無相關(直線)，看起來沒有政黨明顯是民主進步黨的側翼  
> (2)各政黨與韓國瑜
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E6%94%BF%E9%BB%A8%E5%BE%97%E7%A5%A8%E7%8E%87%E8%88%87%E9%9F%93%E5%BE%97%E7%A5%A8%E7%8E%87%E9%97%9C%E4%BF%82%E5%9C%96.PNG)  
> :bulb:中國國民黨與韓國瑜得票率高度正相關，斜率更加接近1，比民主進步黨與蔡英文的關係更強烈  
> :bulb:中國民主黨與蔡英文得票率高度負相關  
> :bulb:其餘政黨皆與韓國瑜得票率無相關(直線)，看起來沒有政黨明顯是中國民主黨的側翼  
----
## ChangeLog  
1. 2020/03/22 首次上傳:2020台灣正副總統得票率視覺化分析.ipynb  
2. 2020/03/25 加入不分區立委分析  
----
## Review  
這是我第一次上傳資料分析作品，動機為2020大選後看到許多人在分析選情，自己也下載政府開放式資料來分析～  
也是第一次接觸與應用了geopandas這個套件，多了一個資料視覺化的方式，感謝以下兩個網站的教學！  
也是第一次寫了完整的README，圖片還太大要再縮小、敘述與敘述可能不太清楚，還有好多地方待改進。  
感覺可以將縣市名稱標上、再加上艱難選區分析等等，以後有空再慢慢更新囉！  
----
## Resources
* [2020總統(副總統)與立委資料](https://db.cec.gov.tw/histMain.jsp?voteSel=20200101A1)  
* [台灣地理資料](https://data.gov.tw/dataset/7438)   
----
## Thanks
* [From Pandas to GeoPandas - 地理資料處理與分析](https://www.slideshare.net/ssusereaac8d/from-pandas-to-geopandas?next_slideshow=1)
* [Let’s make a map! Using Geopandas, Pandas and Matplotlib to make a Choropleth map](https://towardsdatascience.com/lets-make-a-map-using-geopandas-pandas-and-matplotlib-to-make-a-chloropleth-map-dddc31c1983d)
