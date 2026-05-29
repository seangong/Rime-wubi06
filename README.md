# 新世纪五笔+拼音

macOS 版 鼠须管 新世纪五笔+拼音配置。 

1、 新世纪五笔 支持拼音反查。 

2、 五笔与拼音 二合一，五笔输入时遇到不会输入的字，直接输入拼音即可，不用在五笔和拼音之间切换。


# 鼠须管词库挂载配置

1、点击 输入法 ---> 用户设定，会打开输入法配置目录。

2、将下载的字库解压到这个目录，字库不要创建子目录放字库。直接将 yml 文件全扔到 ~/Library/Rime 目录即可。

3、如果不想覆盖自己的配置，在 default.custom.yaml 配置文件加上 wubi06_pinyin 即可。

```yml
# default.custom.yaml
# save it to:
#   ~/.config/ibus/rime  (linux)
#   ~/Library/Rime       (macos)
#   %APPDATA%\Rime       (windows)

patch:
  schema_list:
    - schema: wubi06_pinyin   # 新世纪五笔+拼音
    - schema: clover          # 四叶草拼音输入法
    - schema: pinyin_simp
```

4、重启部署即可。