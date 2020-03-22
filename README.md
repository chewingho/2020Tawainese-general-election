# 2020 Tawainese-general-election
----
## Description
> 透過政府開放式資料:  
> 1.2020總統(副總統)選舉資訊(xls)  
> 2.台灣地理資訊(shp)  
> 繪製台灣總統得票率藍綠版圖、進行鐵票區分析
----
## Process
1. 用正規表示式匯入所需投票資訊檔案  
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E6%8A%95%E7%A5%A8%E7%8E%87%E4%B8%8B%E8%BC%89%E8%B3%87%E6%96%99%E5%A4%BE%E4%B9%8B%E6%AA%94%E6%A1%88.PNG)
2. 透過Function清理投票資訊  
> (1)整理前  
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E7%B8%BD%E7%B5%B1%E6%8A%95%E7%A5%A8%E7%8E%87%E5%8E%9F%E5%A7%8B%E8%B3%87%E6%96%99.PNG)  
> (2)整理後  
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E7%B8%BD%E7%B5%B1%E6%8A%95%E7%A5%A8%E7%8E%87%E8%BD%89%E6%8F%9B%E5%BE%8C.PNG)
3. 匯入shp檔，整理地理資訊  
> (1)整理前  
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E5%9C%B0%E7%90%86%E5%8E%9F%E5%A7%8B%E8%B3%87%E6%96%99.PNG)  
> (2)整理後  
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E5%9C%B0%E7%90%86%E8%B3%87%E6%96%99%E8%BD%89%E6%8F%9B%E5%BE%8C.PNG)
4. 資料縣市與鄉鎮市區得票率視覺化  
> 蔡英文得票率由高到低顏色對應為綠->白->藍  
(1)縣市  
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E7%B8%A3%E5%B8%82%E7%B8%BD%E7%B5%B1%E8%97%8D%E7%B6%A0%E7%89%88%E5%9C%96.PNG)  
(2)鄉鎮市區  
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E9%84%89%E9%8E%AE%E5%B8%82%E5%8D%80%E7%B8%BD%E7%B5%B1%E8%97%8D%E7%B6%A0%E7%89%88%E5%9C%96.PNG)
5. 高票地區與中立地區分析  
> 中立選區為(蔡得票率-韓得票率)相差小之區域  
![image](https://github.com/chewingho/2020Tawainese-general-election/blob/master/%E9%AB%98%E7%A5%A8%E5%8D%80%E8%88%87%E4%B8%AD%E7%AB%8B%E5%8D%80.PNG)
----
## ChangeLog  
1. 2020/03/22 首次上傳:2020台灣正副總統得票率視覺化分析.ipynb
----
## Resources
[2020總統(副總統)選舉資料](https://db.cec.gov.tw/histMain.jsp?voteSel=20200101A1)  
[台灣地理資料](https://data.gov.tw/dataset/7438)   
----
## Thanks
[From Pandas to GeoPandas - 地理資料處理與分析](https://www.slideshare.net/ssusereaac8d/from-pandas-to-geopandas?next_slideshow=1)
