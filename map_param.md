# Gmappingのパラメータ解説

以下のファイルから編集できます

raspicat_ws/src/raspicat_slam_navigation/launch/slam_remote_pc.launch
## オドメトリ誤差

* param name="srr" value="0.03"

    直進１mで生じる道のりの誤差許容量

* param name="srt" value="0.04"

    回転1radで生じる道のりの誤差許容量

* param name="str" value="0.1"

    直進1mで生じる向きの誤差許容量

* param name="stt" value="0.1"

    回転1radで生じる向きの誤差許容量


## 追加パラメータ
* param name="occ_thresh" value="0.25"
  
    セルが障害物かそうでないかを決定する閾値。

    グリッドセルで表現された各セルの値がこの値以上であれば障害物であると判断

## その他

* param name="map_update_interval" value="1.0"

    マップをアップデートする頻度(s)


* param name="maxUrange" value="100.0"

    レーザーの最大使用範囲　
    この値でトリミングされる


* param name="particles" value="120"

    フィルタ内の粒子の数


* param name="iterations" value="5"

    スキャンマッチングの回数


* param name="linearUpdate" value="0.2"

    ロボットが値移動するたびにスキャン

* param name="angularUpdate" value="0.2"

    ロボットがここまで回転するたびにスキャン

* param name="temporalUpdate" value="0.5"

    最後に処理されたスキャンが更新時間（秒単位）よりも古い場合は、スキャン


## 参考
* http://wiki.ros.org/gmapping
* http://rosrosrosrosros.blogspot.com/2013/09/
* https://sy-base.com/myrobotics/ros/gmapping/


