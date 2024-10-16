---
title: 其他函数
aliases: ['/docs-cn/dev/functions-and-operators/miscellaneous-functions/','/docs-cn/dev/reference/sql/functions-and-operators/miscellaneous-functions/']
---

# 其他函数

TiDB 支持使用 MySQL 5.7 中提供的大部分[其他函数](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html)。

## 支持的函数

| 函数名 | 功能描述  |
|:------|:-----------|
| [`ANY_VALUE()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_any-value) | 在 `ONLY_FULL_GROUP_BY` 模式下，防止带有 `GROUP BY` 的语句报错  |
| [`BIN_TO_UUID()`](https://dev.mysql.com/doc/refman/8.0/en/miscellaneous-functions.html#function_bin-to-uuid) | 将通用唯一识别码 (UUID) 从二进制格式转换为文本格式  |
| [`DEFAULT()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_default)  | 返回表的某一列的默认值 |
| [`INET_ATON()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_inet-aton)  | 将 IP 地址转换为数值   |
| [`INET_NTOA()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_inet-ntoa)  | 将数值转换为 IP 地址   |
| [`INET6_ATON()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_inet6-aton)  | 将 IPv6 地址转换为数值   |
| [`INET6_NTOA()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_inet6-ntoa)  | 将数值转换为 IPv6 地址  |
| [`IS_IPV4()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_is-ipv4)   | 判断参数是否为 IPv4 地址   |
| [`IS_IPV4_COMPAT()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_is-ipv4-compat)    | 判断参数是否为兼容 IPv4 的地址   |
| [`IS_IPV4_MAPPED()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_is-ipv4-mapped)    | 判断参数是否为 IPv4 映射的地址   |
| [`IS_IPV6()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_is-ipv6)    | 判断参数是否为 IPv6 地址    |
| [`NAME_CONST()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_name-const)  | 可以用于重命名列名  |
| [`SLEEP()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_sleep)  | 让语句暂停执行几秒时间 |
| [`UUID()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_uuid)  | 返回一个通用唯一识别码 (UUID)  |
| [`UUID_TO_BIN()`](https://dev.mysql.com/doc/refman/8.0/en/miscellaneous-functions.html#function_uuid-to-bin) | 将 UUID 从文本格式转换为二进制格式  |
| [`VALUES()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_values)  | 定义 `INSERT` 语句使用的值  |

## 不支持的函数

| 函数名 | 功能描述  |
|:------|:-----------|
| [`UUID_SHORT()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_uuid-short)  | 基于特定假设提供唯一的 UUID，目前这些假设在 TiDB 中不存在，详见 [TiDB #4620](https://github.com/pingcap/tidb/issues/4620) |
| [`MASTER_WAIT_POS()`](https://dev.mysql.com/doc/refman/5.7/en/miscellaneous-functions.html#function_master-pos-wait)  | 与 MySQL 同步相关 |
