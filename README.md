# 基于zookeeper实现分布式锁
1.分布式锁产生的背景：
  由于服务的集群部署，导致了多个jvm之间的数据不能共享，保持各自的独立性。为了共享数据，保证数据的唯一性，需要使用分布式锁方案
2.分布式锁解决方案
  a.基于zookeeper实现分布式锁
  b.基于redis实现分布式锁
  c.基于数据库实现分布式锁
3.本文基于zk实现分布式锁，原理是利用zk的临时节点的特性实现的。
