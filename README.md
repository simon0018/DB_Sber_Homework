# DB_Sber_Homework
Согласно теореме CAP к какой части вы можете отнести СУБД:
* DragonFly
* ScyllaDB
* ArenadataDB
## DrafonFly
Согласно информации на сайте компании Dragonfly "Dragonfly is **architected to scale vertically** on a single machine, saving teams the cost and complexity of managing a multi-node cluster" таким образом он не Partition tolerance

## Scylla DB
Согласно документации [Scylla Documentation](https://docs.scylladb.com/stable/architecture/architecture-fault-tolerance.html) ScyllaDB относится к AP
"Scylla chooses availability and partition tolerance over consistency, such that:
* It’s impossible to be both consistent and highly available during a network partition;
* If we sacrifice consistency, we can be highly available"

## ArenaData
