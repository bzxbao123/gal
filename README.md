# HighQuality-GalgameTranslator

## About HighQuality-GalgameTranslator
- 基于Python，用于翻译Galgame提取的特定格式日语文本的机器翻译程序
- 通过建立字典，直接翻译字典内文本，解决机器翻译在翻译部分词语或句子时效果很差的问题
- 如果字典很完善，那么翻译的效果将会十分优秀
- 基于词频统计，可以收录文本内的通用高频词
- 基于词频统计，也可以收录文本内的特殊词

## 依赖库
1. TX机器翻译API
```
pip install --upgrade tencentcloud-sdk-python
```
2. excel读取
```
pip install xlrd
```
3. 日语分词
```
pip install mecab-python3
```

## 提取游戏内文本
- 云翻肋手用于提取游戏文本，目前支持的会社有Bishop、WillPlus、YU-RIS、Kaguya、RealLive、PJADV、AliceSoft
- [云翻肋手V0.7](https://pan.baidu.com/share/init?surl=lTMMkPz9PIlmMQQII-uK-Q)
- 提取码:0z9q
- winhex用于查询游戏文本在文件内的偏移量
- [winhex](https://pan.baidu.com/s/10XaxPtgCZhY5eRxca2t7FQ)
- 提取码:eq2w

## 如何协助完成高质量的Galgame机器翻译
- 协助开发Python翻译脚本
- 使用内置的词频统计工具count_word_frequency.py统计未收录的通用高频词
    - 只会将第二列不为空，即有中文翻译的词加入字典
    - 对于机器翻译完全正确的词语请放在excel的[过滤]页下
- 统计某部作品的专有词
    - 对于某部作品的专有词请放在excel的[特殊]页下
- 协助完成字典内收录词语的翻译