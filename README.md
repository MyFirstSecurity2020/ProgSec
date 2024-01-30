# MyFirstProgSec我的第一堂程式安全課 
- 撰寫與講師:崑山科技大學資工系 + 雲端運算暨資通安全研發中心主任  曾龍老師
- 直播課程連結(Google Meet):上課前20分鐘會公告於此
  - https://meet.google.com/ztf-bcyb-ftf  

# 課程宗旨
- 目的:引導同學了解如何在Linux平台上開發c程式及如何分析程式安全
- 本課程屬於初階的入門課程
- 本課程不是C程式設計,但以範例學習模式快速引導同學掌握C程式設計的核心
- 同學於課後需要在研讀其他教科書或網路資源

# 建議的學習模式
- 拚全力聽到懂 挑戰自己的學習能力
- 後續會有教學錄影提供複習

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
- [1_1.範例學習Linux C程式設計](1-1.md)~~~ 
- [1-2.從原始程式碼到執行檔](1-2.md) ~~~ [[20240128直播錄影]](https://youtu.be/S8uVTIzeYmw)
- [1-3.C程式的記憶體佈局(Memory Layout of C Programs)](1-3.md)
- [1-4.LD_PRELOAD技術](1-4.md) ~~~ [[20240128直播錄影]](https://youtu.be/UgnfeIzjEio)
## 第二單元:Linux 執行檔分析(Linux Binary Analysis)
- [2-1.基本Linux 執行檔分析:file|size|string|hexdump|hd](2-1.md)~~~ [[20240128直播錄影]](https://youtu.be/37Pf9tBa2ww)
- [2-2.Linux 執行檔結構ELF(Executable and Linkable Format)](2-2.md)~~~ [[20240128直播錄影(2-2至2-4錄影)]]()
- [2-3.Linux 執行檔分析:readelf](2-3.md)
- [2-4.Linux 執行檔分析:objdump](2-4.md)
- [延伸閱讀][2-5.Linux 執行檔分析常用工具](2-5.md)
## 第三單元:Linux 組合程式設計(Assembly Language Programming in Linux)
- [3-1.計算機結構|指令集與組合程式](3-1.md)
- [3-2.NASM組合程式語法](3-2.md)
- [3-3.NASM(Netwide Assembler)組合程式設計](3-3.md)
- [3-4.解讀關鍵組合語言: C vs assembly](3-4.md)
## 第四單元:逆向工程入門(Introduction to reverse engineering)
- 4-1.[程式安全:逆向工程|PWN](4-1.md)
- 4-2.gdb逆向工程
- 4-3.radare2逆向工程
- 4-4.ghidra逆向工程
- [4-5.我的第一個PWN實測:Buffer overflow(緩衝區溢位)](4-5.md)

