# MUFG-Data-Science-Champion-Ship-2023

Signate Competition
https://signate.jp/competitions/1088

タスク内容  
二値分類  
クレジットカードの顧客登録情報や決済手段・利用場所といった定量及び定性データを元に分析モデルを構築して、カード不正利用の検知にチャレンジしていただきます。

評価関数  
・精度は、F1Score により評価します。

モデル  
model : Stacking( 
layer_1: XGBoost × 3(max_depth=10 & 10 & 6) , RandomForest × 2(max_depth=20 & 10), NN(hidden_layer=6), KNeighbors, logistic_Regression, RGF  
layer_2: XGBoost × 2(max_depth=6 & 3), RandomForest(max_depth=10), NN(hidden_layer=3)  
layer_3: logistic_Regression , XGBoost(max_depth=10)  
)  
threshold = 0.2 

最終評価  
0.6290615

銅メダル獲得

上位入賞者によるとCatBoostを使用すると高い精度が出るそうです。


