# fullJmh

test harness:
[Code Tools: jmh](http://openjdk.java.net/projects/code-tools/jmh/) 

* JMH is a Java harness for building, running, and analysing nano/micro/milli/macro benchmarks written in Java and other languages targetting the JVM.

also:
[jmh-samples](http://hg.openjdk.java.net/code-tools/jmh/file/tip/jmh-samples/src/main/java/org/openjdk/jmh/samples/)

also:
[Java Performance Tuning Guide](http://java-performance.info/jmh/)

* various tips on improving performance of your Java code

details:

| goal                          | command                                                        | 
| ----------------------------- | -------------------------------------------------------------- | 
| build                         | mvn clean package                                              | 
| jmh help                      | java -jar target/benchmarks.jar -h                             | 
| jmh list tests                | java -jar target/benchmarks.jar -l                             | 
| jmh list subset tests         | java -jar target/benchmarks.jar -l {subset}                    | 
| jmh test run all (with flags) | java -jar target/benchmarks.jar -f 1 -wi 3 -i 2 -tu s          | 
| jmh test run one (with flags) | java -jar target/benchmarks.jar -f 1 -wi 3 -i 2 -tu s {subset} | 
