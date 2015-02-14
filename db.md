# db


## mongodb


## mongoose

https://github.com/LearnBoost/mongoose


another choice is [mongo-skin](https://github.com/kissjs/node-mongoskin)


## migroose

https://github.com/derickbailey/migroose


## sqlite

fts3 or fts4 全文检索

https://github.com/mapbox/node-sqlite3/issues/401

```
var sqlite3 = require('..');
var assert = require('assert');

describe('fts', function() {
    var db;
    before(function(done) {
        db = new sqlite3.Database(':memory:', done);
    });

    it('should create a new fts4 table', function(done) {
        db.exec('CREATE VIRTUAL TABLE t1 USING fts4(content="", a, b, c);', done);
    });
});
```

