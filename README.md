

| 接口                    | 描述                           | 所属类  |
|------------------------|------------------------------|--------|
| XMysql()               | 默认构造函数                    | XMysql |
| ~XMysql()              | 默认析构函数                    | XMysql |
| Init()                 | 初始化Mysql上下文               | XMysql |
| Close()                | 清理Mysql占用的所有资源           | XMysql |
| Connect(const char* host, const char* user, const char* pass, const char* db, unsigned short port=3306, unsigned long flag=0) | 数据库连接建立                | XMysql |
| Query(const char* sql, unsigned long sqlLen = 0) | 执行sql语句                    | XMysql |
| Options(enum mysql_option option, const void* arg) | Mysql参数或属性设置              | XMysql |
| SetConnectTimeout(int sec) | 设置连接超时阀值                  | XMysql |
| SetReconnect(bool isre = true) | 自动重连，默认不启动              | XMysql |
| StoreResult()          | 返回全部结果集                   | XMysql |
| UseResult()            | 开始接收结果集，通过Fetch获取       | XMysql |
| FreeResult()           | 释放结果集占用的空间              | XMysql |
| FetchRow()             | 获取一行数据                    | XMysql |
| GetInsertSql(map<string, XData> kv, string table) | 自动根据map生成insert SQL语句   | XMysql |
| Insert(map<string, XData> kv, string table) | 插入二进制数据                  | XMysql |
| InsertBin(map<string, XData> kv, string table) | 插入二进制数据                  | XMysql |
| GetUpdateSql(map<string, XData> kv, string table, string where) | 获取Update数据的sql语句        | XMysql |
| Update(map<string, XData> kv, string table, string where) | 修改表二进制数据               | XMysql |
| UpdateBin(map<string, XData> kv, string table, string where) | 修改表二进制数据               | XMysql |
| StartTransaction()     | 开始事务                       | XMysql |
| StopTransaction()      | 结束事务                       | XMysql |
| Commit()               | 事务提交                       | XMysql |
| Rollback()             | 回滚                         | XMysql |
