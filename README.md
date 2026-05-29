# 新世纪五笔+拼音

macOS 版 鼠须管 新世纪五笔+拼音配置。 

1、新世纪五笔，86版本五笔，86版本简入繁出。
2、支持五笔和拼音混输，2 码默认是五笔，不会触发拼音输入。
3、拼音输入超过 3 码，会自动切换到拼音输入模式，不需要特殊键触发。
4、使用 Ctrl + `（即 1 左侧那个键） 触发拼音反查五笔。


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
    - schema: wubi86_pinyin   # 新世纪五笔+拼音
    - schema: clover          # 四叶草拼音输入法，如果你用四叶草，否则删除本行
    - schema: pinyin_simp
```

4、重启部署即可。