# Gmappingのパラメータ解説
## オドメトリ誤差

* param name="srr" value="0.03"


## 追加パラメータ
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


