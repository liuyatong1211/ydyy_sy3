根据网上的改写，基础功能：当天当地天气，未来六天天气，PM2.5有关信息没有。


SharedPreferences settings= getSharedPreferences("setting", Context.MODE_PRIVATE);


Context.MODE_PRIVATE：为默认操作模式，代表该文件是私有数据，只能被应用本身访问，在该模式下，写入的内容会覆盖原文件的内容，如果想把新写入的内容追加到原文件中。可以使用Context.MODE_APPEND；

Context.MODE_APPEND：模式会检查文件是否存在，存在就往文件追加内容，否则就创建新文件；

Context.MODE_WORLD_READABLE和Context.MODE_WORLD_WRITEABLE用来控制其他应用是否有权限读写该文件：
MODE_WORLD_READABLE：表示当前文件可以被其他应用读取；
MODE_WORLD_WRITEABLE：表示当前文件可以被其他应用写入。
