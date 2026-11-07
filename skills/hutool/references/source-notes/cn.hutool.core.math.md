# cn.hutool.core.math

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.math.Arrangement` | `Iterable<String[]> iterate(int m)` | 返回一个排列的迭代器 |
| `cn.hutool.core.math.Arrangement` | `List<String[]> select()` | 全排列选择（列表全部参与排列） |
| `cn.hutool.core.math.Arrangement` | `List<String[]> select(int m)` | 从当前数据中选择 m 个元素，生成所有「不重复」的排列（Permutation）。 说明： 不允许重复选择同一个元素（即经典排列 A(n, m)） 结果中不会出现 ["1","1"] 这种重复元素的情况 顺序敏感，因此 ["1","2"] 与 ["2","1"] 都会包含 数量公式： |
| `cn.hutool.core.math.Arrangement` | `List<String[]> selectAll()` | 生成当前数据的全部不重复排列（长度为 1 至 n 的所有排列）。 说明： 不允许重复选择元素（无 ["1","1"]，无 ["2","2","3"] 这种） 包含所有长度 m=1..n 的排列 总数量为 A(n,1) + A(n,2) + ... + A(n,n) 举例（datas = ["1","2","3"]）： |
| `cn.hutool.core.math.Arrangement` | `long count(int n)` | 计算排列数，即A(n, n) = n! |
| `cn.hutool.core.math.Arrangement` | `long count(int n,int m)` | 计算排列数，即A(n, m) = n!/(n-m)! |
| `cn.hutool.core.math.Arrangement` | `long countAll(int n)` | 计算排列总数，即A(n, 1) + A(n, 2) + A(n, 3)... |
| `cn.hutool.core.math.BitStatusUtil` | `boolean has(int states,int stat)` | 判断是否含有状态 |
| `cn.hutool.core.math.BitStatusUtil` | `int add(int states,int stat)` | 增加状态 |
| `cn.hutool.core.math.BitStatusUtil` | `int clear()` | 清空状态就是0 |
| `cn.hutool.core.math.BitStatusUtil` | `int remove(int states,int stat)` | 删除一个状态 |
| `cn.hutool.core.math.Calculator` | `double calculate(String expression)` | 按照给定的表达式计算 |
| `cn.hutool.core.math.Calculator` | `double conversion(String expression)` | 计算表达式的值 |
| `cn.hutool.core.math.Combination` | `BigInteger countBig(int n,int m)` | 计算组合数 C(n, m) 的 BigInteger 精确版本。 使用逐步累乘除法（非阶乘）保证不溢出、性能好。 数学定义： C(n, m) = n! / (m! (n - m)!) 优化方式： 1. 利用对称性 m = min(m, n-m) 2. 每一步先乘 BigInteger，再除以当前 i，保证数值不暴涨 |
| `cn.hutool.core.math.Combination` | `List<String[]> select(int m)` | 组合选择（从列表中选择m个组合） |
| `cn.hutool.core.math.Combination` | `List<String[]> selectAll()` | 全组合 |
| `cn.hutool.core.math.Combination` | `long count(int n,int m)` | 计算组合数，即C(n, m) = n!/((n-m)! * m!) 注意：此方法内部使用 BigInteger 修复了旧版 factorial 的计算错误， 但最终仍以 long 返回，因此当结果超过 long 范围时仍会溢出。 建议使用 #countBig(int, int) 获取精确结果，或使用 #countSafe(int, int) 获取安全 long 版本。 |
| `cn.hutool.core.math.Combination` | `long countAll(int n)` | 计算组合总数，即C(n, 1) + C(n, 2) + C(n, 3)... |
| `cn.hutool.core.math.Combination` | `long countSafe(int n,int m)` | 安全组合数 long 版本。 |
| `cn.hutool.core.math.MathUtil` | `List<String[]> arrangementSelect(String[] datas)` | 全排列选择（列表全部参与排列） |
| `cn.hutool.core.math.MathUtil` | `List<String[]> arrangementSelect(String[] datas,int m)` | 排列选择（从列表中选择n个排列） |
| `cn.hutool.core.math.MathUtil` | `List<String[]> combinationSelect(String[] datas,int m)` | 组合选择（从列表中选择n个组合） |
| `cn.hutool.core.math.MathUtil` | `double centToYuan(long cent)` | 金额分转换为元 |
| `cn.hutool.core.math.MathUtil` | `long arrangementCount(int n)` | 计算排列数，即A(n, n) = n! |
| `cn.hutool.core.math.MathUtil` | `long arrangementCount(int n,int m)` | 计算排列数，即A(n, m) = n!/(n-m)! |
| `cn.hutool.core.math.MathUtil` | `long combinationCount(int n,int m)` | 计算组合数，即C(n, m) = n!/((n-m)! * m!) |
| `cn.hutool.core.math.MathUtil` | `long yuanToCent(double yuan)` | 金额元转换为分 |
| `cn.hutool.core.math.Money` | `BigDecimal getAmount()` | 获取本货币对象代表的金额数。 |
| `cn.hutool.core.math.Money` | `Currency getCurrency()` | 获取本货币对象代表的币种。 |
| `cn.hutool.core.math.Money` | `Money add(Money other)` | 货币加法。 如果两货币币种相同，则返回一个新的相同币种的货币对象，其金额为 两货币对象金额之和，本货币对象的值不变。 如果两货币对象币种不同，抛出java.lang.IllegalArgumentException。 |
| `cn.hutool.core.math.Money` | `Money addTo(Money other)` | 货币累加。 如果两货币币种相同，则本货币对象的金额等于两货币对象金额之和，并返回本货币对象的引用。 如果两货币对象币种不同，抛出java.lang.IllegalArgumentException。 |
| `cn.hutool.core.math.Money` | `Money divide(BigDecimal val)` | 货币除法。 返回一个新的货币对象，币种与本货币对象相同，金额为本货币对象的金额除以除数。 本货币对象的值不变。如果相除后的金额不能转换为整数分，使用缺省的取整模式 DEFAULT_ROUNDING_MODE进行取整。 |
| `cn.hutool.core.math.Money` | `Money divide(BigDecimal val,RoundingMode roundingMode)` | 货币除法。 返回一个新的货币对象，币种与本货币对象相同，金额为本货币对象的金额除以除数。 本货币对象的值不变。如果相除后的金额不能转换为整数分，使用指定的取整模式 roundingMode进行取整。 |
| `cn.hutool.core.math.Money` | `Money divide(double val)` | 货币除法。 返回一个新的货币对象，币种与本货币对象相同，金额为本货币对象的金额除以除数。 本货币对象的值不变。如果相除后的金额不能转换为整数分，使用四舍五入方式取整。 |
| `cn.hutool.core.math.Money` | `Money divideBy(BigDecimal val)` | 货币累除。 本货币对象金额除以除数，并返回本货币对象。 如果相除后的金额不能转换为整数分，使用缺省的取整模式 DEFAULT_ROUNDING_MODE进行取整。 |
| `cn.hutool.core.math.Money` | `Money divideBy(BigDecimal val,RoundingMode roundingMode)` | 货币累除。 本货币对象金额除以除数，并返回本货币对象。 如果相除后的金额不能转换为整数分，使用指定的取整模式 roundingMode进行取整。 |
| `cn.hutool.core.math.Money` | `Money divideBy(double val)` | 货币累除。 本货币对象金额除以除数，并返回本货币对象。 如果相除后的金额不能转换为整数分，使用四舍五入方式取整。 |
| `cn.hutool.core.math.Money` | `Money multiply(BigDecimal val)` | 货币乘法。 返回一个新的货币对象，币种与本货币对象相同，金额为本货币对象的金额乘以乘数。 本货币对象的值不变。如果相乘后的金额不能转换为整数分，使用缺省的取整模式 DEFUALT_ROUNDING_MODE进行取整。 |
| `cn.hutool.core.math.Money` | `Money multiply(BigDecimal val,RoundingMode roundingMode)` | 货币乘法。 返回一个新的货币对象，币种与本货币对象相同，金额为本货币对象的金额乘以乘数。 本货币对象的值不变。如果相乘后的金额不能转换为整数分，使用指定的取整方式 roundingMode进行取整。 |
| `cn.hutool.core.math.Money` | `Money multiply(double val)` | 货币乘法。 返回一个新的货币对象，币种与本货币对象相同，金额为本货币对象的金额乘以乘数。 本货币对象的值不变。如果相乘后的金额不能转换为整数分，则四舍五入。 |
| `cn.hutool.core.math.Money` | `Money multiply(long val)` | 货币乘法。 返回一个新的货币对象，币种与本货币对象相同，金额为本货币对象的金额乘以乘数。 本货币对象的值不变。 |
| `cn.hutool.core.math.Money` | `Money multiplyBy(BigDecimal val)` | 货币累乘。 本货币对象金额乘以乘数，并返回本货币对象。 如果相乘后的金额不能转换为整数分，使用缺省的取整方式 DEFUALT_ROUNDING_MODE进行取整。 |
| `cn.hutool.core.math.Money` | `Money multiplyBy(BigDecimal val,RoundingMode roundingMode)` | 货币累乘。 本货币对象金额乘以乘数，并返回本货币对象。 如果相乘后的金额不能转换为整数分，使用指定的取整方式 roundingMode进行取整。 |
| `cn.hutool.core.math.Money` | `Money multiplyBy(double val)` | 货币累乘。 本货币对象金额乘以乘数，并返回本货币对象。 如果相乘后的金额不能转换为整数分，则使用四舍五入。 |
| `cn.hutool.core.math.Money` | `Money multiplyBy(long val)` | 货币累乘。 本货币对象金额乘以乘数，并返回本货币对象。 |
| `cn.hutool.core.math.Money` | `Money subtract(Money other)` | 货币减法。 如果两货币币种相同，则返回一个新的相同币种的货币对象，其金额为 本货币对象的金额减去参数货币对象的金额。本货币对象的值不变。 如果两货币币种不同，抛出java.lang.IllegalArgumentException。 |
| `cn.hutool.core.math.Money` | `Money subtractFrom(Money other)` | 货币累减。 如果两货币币种相同，则本货币对象的金额等于两货币对象金额之差，并返回本货币对象的引用。 如果两货币币种不同，抛出java.lang.IllegalArgumentException。 |
| `cn.hutool.core.math.Money` | `Money[] allocate(int targets)` | 货币分配。 将本货币对象尽可能平均分配成targets份。 如果不能平均分配尽，则将零头放到开始的若干份中。分配 运算能够确保不会丢失金额零头。 |
| `cn.hutool.core.math.Money` | `Money[] allocate(long[] ratios)` | 货币分配。 将本货币对象按照规定的比例分配成若干份。分配所剩的零头 从第一份开始顺序分配。分配运算确保不会丢失金额零头。 |
| `cn.hutool.core.math.Money` | `String dump()` | 生成本对象内部变量的字符串表示，用于调试。 |
| `cn.hutool.core.math.Money` | `String toString()` | 生成本对象的缺省字符串表示 |
| `cn.hutool.core.math.Money` | `boolean equals(Money other)` | 判断本货币对象与另一货币对象是否相等。 货币对象与另一货币对象相等的充分必要条件是： 金额相同。 币种相同。 |
| `cn.hutool.core.math.Money` | `boolean equals(Object other)` | 判断本货币对象与另一对象是否相等。 货币对象与另一对象相等的充分必要条件是： 另一对象也属货币对象类。 金额相同。 币种相同。 |
| `cn.hutool.core.math.Money` | `boolean greaterThan(Money other)` | 货币比较。 判断本货币对象是否大于另一货币对象。 如果待比较的两个货币对象的币种不同，则抛出java.lang.IllegalArgumentException。 如果本货币对象的金额大于待比较货币对象，则返回true，否则返回false。 |
| `cn.hutool.core.math.Money` | `int compareTo(Money other)` | 货币比较。 比较本货币对象与另一货币对象的大小。 如果待比较的两个货币对象的币种不同，则抛出java.lang.IllegalArgumentException。 如果本货币对象的金额少于待比较货币对象，则返回-1。 如果本货币对象的金额等于待比较货币对象，则返回0。 如果本货币对象的金额大于待比较货币对象，则返回1。 |
| `cn.hutool.core.math.Money` | `int getCentFactor()` | 获取本货币币种的元/分换算比率。 |
| `cn.hutool.core.math.Money` | `int hashCode()` | 计算本货币对象的杂凑值。 |
| `cn.hutool.core.math.Money` | `long getCent()` | 获取本货币对象代表的金额数。 |
| `cn.hutool.core.math.Money` | `void setAmount(BigDecimal amount)` | 设置本货币对象代表的金额数。 |
| `cn.hutool.core.math.Money` | `void setCent(long cent)` | 设置货币的分值。 |
