将结巴分词做成 http 服务。可在 config.json 里修改端口和自定义字典

```
pip install requirements.txt
python start.py
```

所有请求支持 GET POST，所有参数只有sentence为必须，其他都是可选。类型为布尔的参数传了就表示 True，不传表示 False。具体功能参考 [jieba](https://github.com/fxsjy/jieba)
```
/cut?sentence=&cut_all=&HMM=
/cut_for_search?sentence=&HMM=
/posseg_cut?sentence=&HMM=
/tokenize?sentence=&mode=&HMM
```

userdict 下面是我总结的词典
brand.txt 品牌名