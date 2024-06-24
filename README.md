# material_ML_portfolio

このポートフォリオは、高性能な電池につながる材料特性を抽出するために、回帰分析や決定木系モデルを使用したノートブック集です。
各種機械学習モデルの重みや特徴量を解析することを目的としています。

# データファイル
material_feature_df.csv.gz
Material ProjectからLiを含む化合物情報をダウンロードして作成したデータです。

Li_material_featurizer_matminer.csv.gz
material_feature_df.csvから、特徴量作成機であるmatminerを用いて追加した特徴量を含むデータです。

learning_Li_battery_data.csv
整理したデータで、最終的に各種機械学習モデルに読み込む際に使用したデータです。

# ノートブック
make_Li_dataframe.ipynb
Material Projectからデータをダウンロードし、DataFrame形式に変換するためのノートブックです。

material_feature.ipynb
DataFrameに特徴量を追加するためのノートブックです。

battery_data_OLS.ipynb
battery_data_lasso.ipynb
battery_data_ridge.ipynb
battery_data_DecisionTreeRegressor.ipynb
battery_data_randomforest_regressor.ipynb

各種機械学習モデルを用いて予測を行い、重みの可視化を行ったノートブックです。それぞれ以下の方法を使用しています。
- 回帰分析 (OLS)
- Lasso回帰
- Ridge回帰
- 決定木
- ランダムフォレスト
