#  mypkg  
![test]https://(github.com/Kazuma-2932/mypkg/actions/workflows/test.yml/badge.svg)  
talker.pyとlistener.pyというノードを用いて数字を通信し、表示するリポジトリです。  

#  ノードの説明    
 *  talker.py  
    パブリッシャを持つノードで、数字をカウントしてトピック/countupを通じて送信する機能を持つ。  
 *  listener.py  
    サブスクライバを持つノードで、/countupからメッセージをもらって表示する機能を持つ。  
 *  talk_listen.launch/py  
    複数のノード(ここではtalk.pyとlistener.py)を一度に立ち上げるもの。  

#  使い方と結果  
 *  使い方  

 　1. 端末１で以下のコードを入力し、talker.pyを立ち上げる。  

  　``
  　 $ ros2 run mypkg talker  
  　``

 　2. 端末２で以下のコードを入力し、listener.pyを立ち上げる。  

　　``
  　 $ ros2 run mypkg listener  
    ``

 *  結果
  
```
[INFO] [1705142972.437665858] [listener]: Listen: 30  

[INFO] [1705142972.931000807] [listener]: Listen: 31  

[INFO] [1705142973.430993508] [listener]: Listen: 32 

[INFO] [1705142973.930983991] [listener]: Listen: 33  

[INFO] [1705142974.431424769] [listener]: Listen: 34  

[INFO] [1705142974.930150495] [listener]: Listen: 35  

[INFO] [1705142975.430611720] [listener]: Listen: 36  

[INFO] [1705142975.930991267] [listener]: Listen: 37  

[INFO] [1705142976.430785924] [listener]: Listen: 38  

[INFO] [1705142976.931112156] [listener]: Listen: 39  

[INFO] [1705142977.431388473] [listener]: Listen: 40  
```

#  必要なソフトウェア  
 ROS2 foxy  

#  テスト環境  
 Ubuntu 20.04.6 LTS  

#  権利関係  
　*  このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます.  
  *  このパッケージのコードは，下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを，本人の許可を得て自身の著作としたものです．  
      *  https://ryuichiueda.github.io/my_slides/robosys_2022/lesson8.html#/  
      *  https://ryuichiueda.github.io/my_slides/robosys_2022/lesson9.html#/  
      *  https://ryuichiueda.github.io/my_slides/robosys_2022/lesson10.html#/  
  *  ©2023 Kazuma-2932  
