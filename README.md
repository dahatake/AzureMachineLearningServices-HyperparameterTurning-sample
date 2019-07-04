# Azure Machine Learning services Samples

`docs.microsoft.com` のサンプルに、もう少し各トピックを加えたものです。

https://docs.microsoft.com/ja-jp/azure/machine-learning/service/samples-notebooks


# ファイルの説明
 - 0.config.ipynb

Azure Machine Learning services の Workspace の作成用。執筆時点 (2019/7/3)で、Azure Portal から Workspace を作成すると、CPU / GPU のデフォルトのコンピューターが設定されない。そのため、Python SDK からの方を推奨します。

参考: Azure Machine Learning service ワークスペースを作成する:

https://docs.microsoft.com/ja-jp/azure/machine-learning/service/setup-create-workspace

 - 1.train-hyperparameter-tune-deploy-with-keras.ipynb

Azure Machine Learning services の  Hyperparameters Turning を使ったサンプル。 `HyperDrive` は、`Automated Machine Learning` の機能と切り離して利用ができます。執筆時点 (2019/7/3) 時点だと、Automated Machine Learning は、Deep Learning には使えないため、単独のサンプルとして。

  - MNIST
  - Keras + Tensorflow
  - Neural Network はコードから作成
  - GPU 利用前提
    - NCv3 (Volta)
    - 複数 GPU コア利用
    - TensorCore を使うための `Automatic Mixed Precision` の有効化
    https://docs.nvidia.com/deeplearning/frameworks/tensorflow-user-guide/index.html

  参考: https://docs.microsoft.com/ja-jp/azure/machine-learning/service/how-to-tune-hyperparameters

# 手順

1. Azure の Subscription を作成

Azure Machine Learning services を利用するために必要です。

無料トライアル: https://azure.microsoft.com/ja-jp/free/

2. Azure Notebook にログイン

こちらです。

https://notebooks.azure.com/

3. Azure Notebook で Github Clone

手順はこちら。

https://docs.microsoft.com/ja-jp/azure/notebooks/quickstart-clone-jupyter-notebook

後は 0->１と実行ください😊

## 参考

Azure Machine Learning Services ドキュメント:

https://docs.microsoft.com/ja-jp/azure/machine-learning/service/

Azure Notebooks のドキュメント:

https://docs.microsoft.com/ja-jp/azure/notebooks/