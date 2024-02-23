# MyFirstProgSec我的第一堂程式安全課 
- 講師:崑山科技大學資工系 + 雲端運算暨資通安全研發中心主任  曾龍老師
- 直播課程連結(Google Meet):上課前20分鐘會公告於此
# 作業說明 Google Meet 
- https://meet.google.com/zjs-otzh-vww
# 課程宗旨
- 目的:引導同學了解如何在Linux平台上開發c程式及如何分析程式安全
- 本課程屬於初階的入門課程
- 本課程不是C程式設計,但以範例學習模式快速引導同學掌握C程式設計的核心
- 同學於課後需要在研讀其他教科書或網路資源

# 建議的學習模式
- 拚全力聽到懂 挑戰自己的學習能力
- 後續會有教學錄影提供複習

# 證書發放標準:繳交PPT簡報(2024.2.15)
- 簡報內容:證明你具備底下能力與知識
  - 1.可以在Linux平台上完成C程式開發(可以挑選重要的範例展示)
  - 2.熟悉Linux Binary的基本分析(readelf, objdump等工具的使用)
  - 3.對組合語法的熟悉度(可以使用Linux nasm開發簡單的組合程式與基本組合程式解析)
    - 可以參考推薦書籍的範例,說明其語法
  - 4.逆向工程的技術:至少包括
    - 4.1.使用radare 2 逆向出組合程式與分析
    - 4.2.使用Ghidra 逆向出c/c++程式與分析
  - 5.PWN 程式漏洞的安全測試
- 標準:
  - 通過的基本條件:課堂上範例的練習(可以挑選重要的範例展示)
  - 推薦的優秀標準:
    - 1.自行上網閱讀資料與測試
    - 2.自己完成的分析
    - 3.使用自己的簡報加上直接展示畫面 ==> 錄下你的成長紀錄 ==> [OBS](https://obsproject.com/)錄影
- 有沒有範本可以參考?
  - `自己訂下你認為的最好架構,展示妳的所學` 這是很重要的練習
  - `走自己的路 + 講自己精通的內容 + 以後奉獻你的所長` 是本課程衷心希望
  - 講師會找時間(某個晚上)(直播加錄影)提供你一些提示 
- 持續不斷精進自己的資安戰鬥力 是要 一步一步認真努力的 ~~ 加油
  - 這門課程對高中職同學而言屬於較艱深課程,可以和同學一起學習與討論(但不能抄襲別人的作業)
  - `用自己的話 說清楚 你會的`是很重要的訓練
  - 剛開始會比較生硬 堅持成長 
  - 熟悉後 你會很有自信 ~~你可以的 ~~我看好你

# 學生預先作業:Linux測試環境下載與建置
- 本課程使用虛擬化技術(在Windows作業系統上安裝Virtualbox,然後匯入linux)學習linux
- 教學環境:本課程使用虛擬機匯入Kali Linux進行教學
  - 步驟1:在你的電腦下載 [virtual box](https://www.virtualbox.org/wiki/Downloads) 並安裝完成 [Virtualbox安裝:YOUTUBE影片](https://youtu.be/FC0CX71aGnc)
  - 步驟2:點選資料下載點, 下載Linux系統
    - Python會用到的Ubuntu Linux 18.04 LTS(已安裝好pwntools)  [下載點](https://drive.google.com/file/d/1aP-qCFP6jKsGYXtKy9ahwZleQSENEi7C/view?usp=sharing)
  - 步驟3:匯入你要用的linux  [[YOUTUBE教學錄影]](https://youtu.be/GTpQR7fZcwE)
- 請預先申請你的 [github](https://github.com/)  ~ 請上網Google 一下申請辦法

# 課程內容
## 第一單元:Linux C程式設計(Linux C Programming)
- [1_1.範例學習Linux C程式設計](1-1.md)~~~ [20240128第一堂教學錄影](https://youtu.be/EPMsu_SoLPE) ~~~[20240128第二堂教學錄影](https://youtu.be/BFYjyARU9Ec)
- [1-2.從原始程式碼到執行檔](1-2.md) ~~~ [[20240128直播錄影]](https://youtu.be/S8uVTIzeYmw)
- [1-3.C程式的記憶體佈局(Memory Layout of C Programs)](1-3.md)
- [1-4.LD_PRELOAD技術](1-4.md) ~~~ [[20240128直播錄影]](https://youtu.be/UgnfeIzjEio)
## 第二單元:Linux 執行檔分析(Linux Binary Analysis)
- [2-1.基本Linux 執行檔分析:file|size|string|hexdump|hd](2-1.md)~~~ [[20240128直播錄影]](https://youtu.be/37Pf9tBa2ww)
- [2-2.Linux 執行檔結構ELF(Executable and Linkable Format)](2-2.md)~~~ [[20240128直播錄影(2-2至2-4錄影)]](https://youtu.be/OHRuoDxbd_M)
- [2-3.Linux 執行檔分析:readelf](2-3.md)
- [2-4.Linux 執行檔分析:objdump](2-4.md)
- [延伸閱讀][2-5.Linux 執行檔分析常用工具](2-5.md)
## 第三單元:Linux 組合程式設計(Assembly Language Programming in Linux)
- [3-1.計算機結構|指令集與組合程式](3-1.md) ~~[[20240131直播錄影]](https://youtu.be/-Vh8nqHn33s)
- [3-2.NASM組合程式語法(參考用)](3-2.md)
- [3-3.NASM(Netwide Assembler)組合程式設計](3-3.md)
  - [[20240131直播錄影:NASM]](https://youtu.be/VoZ9XQEzluU) [[20240131直播錄影:GDB分析]](https://youtu.be/bJQfjVrsV1E)
- [3-4.解讀關鍵組合語言: C vs assembly](3-4.md)
## 第四單元:逆向工程入門(Introduction to reverse engineering)
- [4-1.程式安全:逆向工程|PWN](4-1.md)
- [4-2.gdb逆向工程](4-2.md)
- [4-3.radare2逆向工程(執行檔 ==> 組合語言)](4-3.md)~~[[20240131直播錄影]](https://youtu.be/-122s4qgdM4)
- [4-4.ghidra逆向工程(執行檔 ==> C/C++)](4-4.md)  ~~[[20240131直播錄影]](https://youtu.be/64xacDMWjKE)
- [4-5.我的第一個PWN實測:Buffer overflow(緩衝區溢位)](4-5.md) ~~[[20240131直播錄影]](https://youtu.be/YiBml_ypUo8)

