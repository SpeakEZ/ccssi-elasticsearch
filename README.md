## Common Core State Standards Initiative

Load the JSON of the educational standard and put up on [Amazon
Elasticsearch Service](http://aws.amazon.com/elasticsearch-service).

See the project http://github.com/ashawley/ccssi-xml for how to
convert the CCSSI XML data to JSON.

### Usage

Requires [SBT](http://www.scala-sbt.org/download.html) to compile and
run the system.

The application accepts one or more JSON files as argument(s) of the
`run` target of SBT.

    > run src/main/json/math.json src/main/json/ela-literacy.json
    [info] Running ccssi.Main src/main/json/math.json
              src/main/json/ela-literacy.json
    health      status  index           pri rep docs.count docs.deleted store.size pri.store.size
    green       open    ccssi-1.1         5   1
    DeleteIndex was acknowledged: true
    Elastic endpoint is Volcano
    Mappping was acknowledged: true
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ..
    ERROR: File items (517) did not equal index count (516)
    Completed src/main/json/math.json with 516 items
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    ....................................................................
    .
    ERROR: File items (1050) did not equal index count (1026)
    Completed src/main/json/ela-literacy.json with 1026 items
    File count: 2
    FINISHED
    [success] Total time: 32 s, completed June 31, 2016 4:53:24 PM
