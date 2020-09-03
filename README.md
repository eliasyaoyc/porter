## Porter 
Porter is a distributed MySQL binlog syncer based on raft. Porter can act as a slave to the real master. 
Porter has the following key featues:
* MySQL replication protocol compatibility,pull the binlog files from the Mysql master through gtid mode.
* High available ,porter uses Raft to support High available,The binlog data written to the porter cluster is guaranteed to be consistent between multiple nodes,
and the order of binlog event is exactly the the same as that on the master
### Overview

### Requirements

### Quick Start

### License
```
Copyright (c) 2020 YunLSP+

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

### Acknowledgments
* Thanks [etcd](https://github.com/etcd-io/etcd) for providing raft library.
* Thanks [go-mysql](https://github.com/siddontang/go-mysql) for providing mysql replication protocol parser.
* Thanks [kingbus](https://github.com/flike/kingbus) for providing ideas.
* Thanks [misselvexu](https://github.com/misselvexu) give me support and enough free to complete it.