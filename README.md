# redis-project
一个 redis 项目，主要是熟悉 redis 的开发应用场景

- [x] 实现基于 Session 的登录流程  
- [x] 实现使用 Redis 代替 Session 的登录流程  
- [x] 实现查询缓存：  
    - [x] 增加缓存更新策略  
    - [x] 解决缓存好数据库不一致以及查询的缓存穿透、缓存击穿等问题  
- [ ] 实现秒杀下单：  
    - [x] 使用乐观锁解决超卖线程安全问题
    - [x] 使用悲观锁解决一人一单的超卖线程安全问题
    - [x] 编写简易版 redis 分布式锁解决集群（两个实例。。）下一人一单问题
    - [x] 改进 redis 分布式锁，解决并发下误删锁问题
    - [x] 保证原子性操作，使用 Lua 脚本释放锁
    - [x] 使用 Redisson 的分布式锁代替简易版的 redis 分布式锁