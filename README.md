# Wizardry Online クラスアドバンスメント シミュレータ


##データ

###クラスアドバンスメントデータJSONファイルフォーマット

####サンプル

```
{
	"name": "BIS",
	"boards": [
		{
			"name": "スタンダード",
			"capacity": 50000,
			"skills": [
				{
					"type": "status",
					"label": "火属性特化",
					"efficiency": "0.5",
					"description": "火属性魔法の与ダメージを0.5%増加する。",
					"tiles": [
						{
							"cost": 1500,
							"x": 3,
							"y": 5
						},
						{
							"cost": 1000,
							"x": 3,
							"y": 6
						}
					]
				},
				{
					"type": "free",
					"tiles": [
						{
							"x": 4,
							"y": 6
						},
						{
							"x": 8,
							"y": 3
						},
						{
							"x": 16,
							"y": 3
						},
						{
							"x": 20,
							"y": 6
						}
					]
				}
			]
		}
	]
}
```

####フォーマットの解説

* name	職業名 string
* boards ボード情報を格納したオブジェクトの配列
  * name ボード名
  * capacity AdPoint使用上限
  * skills 各マスの情報を格納したオブジェクトの配列
    * type マスの種類。free/attack/magic/heal/status/alljob/specialのいずれかの値。
	* label マスの名前
	* efficiency 効果値。「1%」や「0.3秒」など習得することによって得られる数値。
	* description 説明。
	* tiles そのマスが配置されている位置と消費AdPointを格納したオブジェクトの配列

##THANKS

###データ校正
* [@renkonq](https://twitter.com/renkonq)
* [@Sancho_dayo](https://twitter.com/Sancho_dayo)
* [@wasa_san](https://twitter.com/wasa_san)

###データ作成
* FIG
  * [@chil0423](https://twitter.com/chil0423)

##Wizardry Online について

[Wizardry Online](http://liberal.wizardry-online.jp/)

>"Wizardry Online(R)" of GMO Gamepot Inc. All rights reserved.
>Wizardry Renaissance TM (C) 2009 GMO Gamepot Inc. All rights reserved
