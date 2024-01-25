# MyFirstProgSec我的第一堂程式安全課 

# 學生預先作業:Linux測試環境下載與建置
- 本次課程使用虛擬化技術(在Windows作業系統上安裝Virtualbox,然後匯入linux)學習linux
- 自建實體教學環境:本課程使用虛擬機匯入Kali Linux進行教學
  - 步驟1:在你的電腦下載 [virtual box](https://www.virtualbox.org/wiki/Downloads) 並安裝完成 [Virtualbox安裝:YOUTUBE影片](https://youtu.be/FC0CX71aGnc)
  - 步驟2:點選資料下載點, 下載Linux系統
    - Python會用到的Ubuntu Linux 18.04 LTS(已安裝好pwntools)  [下載點](https://drive.google.com/file/d/1aP-qCFP6jKsGYXtKy9ahwZleQSENEi7C/view?usp=sharing)
  - 步驟3:匯入你要用的linux  [[YOUTUBE教學錄影]](https://youtu.be/GTpQR7fZcwE)
- 請預先申請你的 [github](https://github.com/)  ~ 請上網Google 一下申請辦法
# 課程內容
## 第一單元:Linux C程式設計(Linux C Programming)
- 1_1.範例學習Linux C程式設計
- 1-2.從原始程式碼到執行檔
- 1-3.C程式的記憶體佈局(Memory Layout of C Programs)
- 1-4.LD_PRELOAD技術
## 第二單元:Linux 執行檔分析(Linux Binary Analysis)
- [2-1.基本Linux 執行檔分析:file|size|string|hexdump|hd](2-1.md)
- [2-2.Linux 執行檔結構ELF(Executable and Linkable Format)](2-2.md)
- [2-3.Linux 執行檔分析:readelf](2-3.md)
- [2-4.Linux 執行檔分析:objdump](2-4.md)
- [延伸閱讀]2-5.Linux 執行檔分析常用工具
## 第三單元:Linux 組合程式設計(Assembly Language Programming in Linux)
- 3-1.計算機結構|指令集與組合程式
- [3-2.NASM(Netwide Assembler)組合程式設計](3-2.md)
- 3-3.NASM組合程式語法
- 3-4.解讀關鍵組合語言: C vs assembly
## 第四單元:逆向工程入門(Introduction to reverse engineering)
- 4-1.逆向工程
- 4-2.objdump逆向工程
- 4-3.gdb逆向工程
- 4-4.radare2逆向工程
- 4-5.ghidra逆向工程

