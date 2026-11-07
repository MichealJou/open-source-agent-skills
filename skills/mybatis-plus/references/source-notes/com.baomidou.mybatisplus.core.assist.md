# com.baomidou.mybatisplus.core.assist

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.assist.ISqlRunner` | `E selectPage(E page,String sql,Object... args)` | 分页查询 |
| `com.baomidou.mybatisplus.core.assist.ISqlRunner` | `List<Map<String, Object>> selectList(String sql,Object... args)` | 根据sql查询Map结果集 SqlRunner.db().selectList("select * from tbl_user where name={0}", "Caratacus") |
| `com.baomidou.mybatisplus.core.assist.ISqlRunner` | `List<Object> selectObjs(String sql,Object... args)` | 根据sql查询一个字段值的结果集 注意：该方法只会返回一个字段的值， 如果需要多字段，请参考#selectList(String, Object...) |
| `com.baomidou.mybatisplus.core.assist.ISqlRunner` | `Map<String, Object> selectOne(String sql,Object... args)` | 获取单条记录 |
| `com.baomidou.mybatisplus.core.assist.ISqlRunner` | `Object selectObj(String sql,Object... args)` | 根据sql查询一个字段值的一条结果 注意：该方法只会返回一个字段的值， 如果需要多字段，请参考#selectOne(String, Object...) |
| `com.baomidou.mybatisplus.core.assist.ISqlRunner` | `boolean delete(String sql,Object... args)` | 执行删除语句 |
| `com.baomidou.mybatisplus.core.assist.ISqlRunner` | `boolean insert(String sql,Object... args)` | 执行插入语句 |
| `com.baomidou.mybatisplus.core.assist.ISqlRunner` | `boolean update(String sql,Object... args)` | 执行更新语句 |
| `com.baomidou.mybatisplus.core.assist.ISqlRunner` | `long selectCount(String sql,Object... args)` | 查询总数 |
