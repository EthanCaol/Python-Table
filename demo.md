

```sh
nohup papermill t5.ipynb t5_run.ipynb --log-output --progress-bar > t5.log 2>&1 &
jupyter nbconvert --to script demo.ipynb
```


TODO
- 修改`best_val_loss = 0.384`到最低误差, 然后按照累计梯度再跑一遍
- 将预训练好的模型上传到Huggingface
- 写推理用的notebook, 并上传到Kaggle
- 在Kaggle上对比赛数据进行推理并提交结果

