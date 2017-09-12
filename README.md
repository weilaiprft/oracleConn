# oracleConn

run a local instance of oracle, using docker is a good option

register ojdbc7
move it to /tmp first

mvn install:install-file -Dfile=/tmp/ojdbc7.jar -DgroupId=com.oracle -DartifactId=ojdbc7 -Dversion=12.1.0 -Dpackaging=jar

mvn clean install

mvn exec:java -Dexec.mainClass="com.wei.OracleJDBCExample"
