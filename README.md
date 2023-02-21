# DB_Sber_Homework
Согласно теореме CAP к какой части вы можете отнести СУБД:
* DragonFly
* ScyllaDB
* ArenadataDB
## DrafonFly
Согласно информации на [сайте](https://dragonflydb.io/) компании Dragonfly

"Dragonfly is **architected to scale vertically on a single machine**, saving teams the cost and complexity of managing a multi-node cluster" таким образом он не Partition tolerance. 

Также "Dragonfly offers the simplest and most **reliable** scale on the market".  
Итого по CAP теорема **DragonFly - CA**

## Scylla DB
Согласно документации [Scylla Documentation](https://docs.scylladb.com/stable/architecture/architecture-fault-tolerance.html) **ScyllaDB относится к AP**  

"Scylla chooses availability and partition tolerance over consistency, such that:
* It’s impossible to be both consistent and highly available during a network partition;
* If we sacrifice consistency, we can be highly available"

## ArenaData
Согласное информации на [сайте](https://arenadata.tech/products/arenadata-db/)

Полное соответствие принципам строгой изоляции транзакции (принципы ACID), т е по мере выполнения транзакций, данные переходят из одного согласованного состояния в другое, то есть транзакция не может разрушить взаимной согласованности данных. 

Также Arenadata DB реализована на кластере из множества (от двух до сотен) серверов и равномерно распределяет нагрузку и данные между ними, которые могут быть масштабированы.  
Итого по CAP теореме **ArenaData - CA**

