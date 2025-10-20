# Toradocu Tutorial

## Compilation process

```shell
auri@av01:~/OneDrive/temp/00-orientacoes/andre-pestana/workspace$ javac -version
javac 1.8.0_341
auri@av01:~/OneDrive/temp/00-orientacoes/andre-pestana/workspace$ git clone https://github.com/aurimrv/toradocu.git
Cloning into 'toradocu'...
remote: Enumerating objects: 14538, done.
remote: Counting objects: 100% (41/41), done.
remote: Compressing objects: 100% (24/24), done.
remote: Total 14538 (delta 16), reused 37 (delta 15), pack-reused 14497 (from 1)
Receiving objects: 100% (14538/14538), 12.31 MiB | 5.73 MiB/s, done.
Resolving deltas: 100% (7600/7600), done.
auri@av01:~/OneDrive/temp/00-orientacoes/andre-pestana/workspace$ ls -l
total 4
drwxrwxr-x 11 auri auri 4096 out 20 10:54 toradocu
auri@av01:~/OneDrive/temp/00-orientacoes/andre-pestana/workspace$ cd toradocu/
auri@av01:~/OneDrive/temp/00-orientacoes/andre-pestana/workspace/toradocu$ ls -l
total 88
-rw-rw-r-- 1 auri auri 20759 out 20 10:54 build.gradle
-rwxrwxr-x 1 auri auri   717 out 20 10:54 clean.sh
drwxrwxr-x 2 auri auri  4096 out 20 10:54 doc
-rwxrwxr-x 1 auri auri   574 out 20 10:54 git-pre-commit-hook.sh
drwxrwxr-x 3 auri auri  4096 out 20 10:54 gradle
-rwxrwxr-x 1 auri auri  5296 out 20 10:54 gradlew
-rw-rw-r-- 1 auri auri  2260 out 20 10:54 gradlew.bat
drwxrwxr-x 2 auri auri  4096 out 20 10:54 lib
-rw-rw-r-- 1 auri auri  1708 out 20 10:54 LICENSE.md
-rw-rw-r-- 1 auri auri  3912 out 20 10:54 nulldereference.ResourceManager_out.json
-rw-rw-r-- 1 auri auri  4534 out 20 10:54 README.md
drwxrwxr-x 2 auri auri  4096 out 20 10:54 scripts
drwxrwxr-x 4 auri auri  4096 out 20 10:54 src
drwxrwxr-x 2 auri auri  4096 out 20 10:54 stats
drwxrwxr-x 4 auri auri  4096 out 20 10:54 tutorial
auri@av01:~/OneDrive/temp/00-orientacoes/andre-pestana/workspace/toradocu$ ./gradlew shadowJar
Downloading https://services.gradle.org/distributions/gradle-4.3.1-bin.zip
.....................................................................
Unzipping /home/auri/.gradle/wrapper/dists/gradle-4.3.1-bin/7yzdu24db77gi3zukl2a7o0xx/gradle-4.3.1-bin.zip to /home/auri/.gradle/wrapper/dists/gradle-4.3.1-bin/7yzdu24db77gi3zukl2a7o0xx
Set executable permissions for: /home/auri/.gradle/wrapper/dists/gradle-4.3.1-bin/7yzdu24db77gi3zukl2a7o0xx/gradle-4.3.1/bin/gradle
Starting a Gradle Daemon (subsequent builds will be faster)
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-gradle-plugin/1.2.21/kotlin-gradle-plugin-1.2.21.pom
Download https://jcenter.bintray.com/de/undercouch/gradle-download-task/3.3.0/gradle-download-task-3.3.0.pom
Download https://plugins.gradle.org/m2/com/github/jengelman/gradle/plugins/shadow/2.0.2/shadow-2.0.2.pom
Download https://plugins.gradle.org/m2/gradle/plugin/com/github/sherter/google-java-format/google-java-format-gradle-plugin/0.7.1/google-java-format-gradle-plugin-0.7.1.pom
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-android-extensions/1.2.21/kotlin-android-extensions-1.2.21.pom
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-compiler-runner/1.2.21/kotlin-compiler-runner-1.2.21.pom
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-compiler-embeddable/1.2.21/kotlin-compiler-embeddable-1.2.21.pom
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-gradle-plugin-api/1.2.21/kotlin-gradle-plugin-api-1.2.21.pom
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-annotation-processing-gradle/1.2.21/kotlin-annotation-processing-gradle-1.2.21.pom
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-stdlib/1.2.21/kotlin-stdlib-1.2.21.pom
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-script-runtime/1.2.21/kotlin-script-runtime-1.2.21.pom
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-reflect/1.2.21/kotlin-reflect-1.2.21.pom
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-build-common/1.2.21/kotlin-build-common-1.2.21.pom
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-daemon-client/1.2.21/kotlin-daemon-client-1.2.21.pom
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-reflect/1.2.21/kotlin-reflect-1.2.21.jar
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-compiler-runner/1.2.21/kotlin-compiler-runner-1.2.21.jar
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-annotation-processing-gradle/1.2.21/kotlin-annotation-processing-gradle-1.2.21.jar
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-compiler-embeddable/1.2.21/kotlin-compiler-embeddable-1.2.21.jar
Download https://plugins.gradle.org/m2/com/github/jengelman/gradle/plugins/shadow/2.0.2/shadow-2.0.2.jar
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-stdlib/1.2.21/kotlin-stdlib-1.2.21.jar
Download https://jcenter.bintray.com/de/undercouch/gradle-download-task/3.3.0/gradle-download-task-3.3.0.jar
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-gradle-plugin-api/1.2.21/kotlin-gradle-plugin-api-1.2.21.jar
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-script-runtime/1.2.21/kotlin-script-runtime-1.2.21.jar
Download https://plugins.gradle.org/m2/gradle/plugin/com/github/sherter/google-java-format/google-java-format-gradle-plugin/0.7.1/google-java-format-gradle-plugin-0.7.1.jar
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-gradle-plugin/1.2.21/kotlin-gradle-plugin-1.2.21.jar
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-daemon-client/1.2.21/kotlin-daemon-client-1.2.21.jar
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-build-common/1.2.21/kotlin-build-common-1.2.21.jar
Download https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-android-extensions/1.2.21/kotlin-android-extensions-1.2.21.jar
Download https://repo1.maven.org/maven2/edu/stanford/nlp/stanford-corenlp/3.6.0/stanford-corenlp-3.6.0.pom
Download https://repo1.maven.org/maven2/org/mdkt/compiler/InMemoryJavaCompiler/1.3.0/InMemoryJavaCompiler-1.3.0.pom
Download https://repo1.maven.org/maven2/com/beust/jcommander/1.69/jcommander-1.69.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-native-platform/0.8.0/nd4j-native-platform-0.8.0.pom
Download https://repo1.maven.org/maven2/org/slf4j/slf4j-simple/1.7.21/slf4j-simple-1.7.21.pom
Download https://repo1.maven.org/maven2/com/github/javaparser/javaparser-core/3.5.4/javaparser-core-3.5.4.pom
Download https://repo1.maven.org/maven2/org/deeplearning4j/deeplearning4j-nlp/0.8.0/deeplearning4j-nlp-0.8.0.pom
Download https://repo1.maven.org/maven2/de/jungblut/common/thomasjungblut-common/1.1/thomasjungblut-common-1.1.pom
Download https://repo1.maven.org/maven2/de/jungblut/math/tjungblut-math/1.3/tjungblut-math-1.3.pom
Download https://repo1.maven.org/maven2/org/deeplearning4j/deeplearning4j-nlp-parent/0.8.0/deeplearning4j-nlp-parent-0.8.0.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-backend-impls/0.8.0/nd4j-backend-impls-0.8.0.pom
Download https://repo1.maven.org/maven2/org/deeplearning4j/deeplearning4j-parent/0.8.0/deeplearning4j-parent-0.8.0.pom
Download https://repo1.maven.org/maven2/com/github/javaparser/javaparser-parent/3.5.4/javaparser-parent-3.5.4.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-backends/0.8.0/nd4j-backends-0.8.0.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j/0.8.0/nd4j-0.8.0.pom
Download https://repo1.maven.org/maven2/com/io7m/xom/xom/1.2.10/xom-1.2.10.pom
Download https://repo1.maven.org/maven2/de/jollyday/jollyday/0.4.7/jollyday-0.4.7.pom
Download https://repo1.maven.org/maven2/javax/json/javax.json-api/1.0/javax.json-api-1.0.pom
Download https://repo1.maven.org/maven2/joda-time/joda-time/2.9/joda-time-2.9.pom
Download https://repo1.maven.org/maven2/com/googlecode/efficient-java-matrix-library/ejml/0.23/ejml-0.23.pom
Download https://repo1.maven.org/maven2/org/glassfish/json/1.0/json-1.0.pom
Download https://repo1.maven.org/maven2/org/apache/commons/commons-math3/3.0/commons-math3-3.0.pom
Download https://repo1.maven.org/maven2/net/sf/trove4j/trove4j/3.0.2/trove4j-3.0.2.pom
Download https://repo1.maven.org/maven2/org/apache/commons/commons-parent/23/commons-parent-23.pom
Download https://repo1.maven.org/maven2/commons-httpclient/commons-httpclient/3.0.1/commons-httpclient-3.0.1.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.pom
Download https://repo1.maven.org/maven2/org/codehaus/jackson/jackson-mapper-asl/1.9.11/jackson-mapper-asl-1.9.11.pom
Download https://repo1.maven.org/maven2/org/htmlparser/htmllexer/2.1/htmllexer-2.1.pom
Download https://repo1.maven.org/maven2/org/apache/logging/log4j/log4j-core/2.1/log4j-core-2.1.pom
Download https://repo1.maven.org/maven2/org/mockito/mockito-all/1.9.5/mockito-all-1.9.5.pom
Download https://repo1.maven.org/maven2/org/apache/mrunit/mrunit/1.0.0/mrunit-1.0.0.pom
Download https://repo1.maven.org/maven2/net/sourceforge/nekohtml/nekohtml/1.9.17/nekohtml-1.9.17.pom
Download https://repo1.maven.org/maven2/org/htmlparser/htmlparser/2.1/htmlparser-2.1.pom
Download https://repo1.maven.org/maven2/org/codehaus/jackson/jackson-core-asl/1.9.11/jackson-core-asl-1.9.11.pom
Download https://repo1.maven.org/maven2/de/l3s/boilerpipe/boilerpipe/1.1.0/boilerpipe-1.1.0.pom
Download https://repo1.maven.org/maven2/org/apache/logging/log4j/log4j/2.1/log4j-2.1.pom
Download https://repo1.maven.org/maven2/de/jungblut/jrpt/jrpt/0.1/jrpt-0.1.pom
Download https://repo1.maven.org/maven2/org/htmlparser/HTMLParserProject/2.1/HTMLParserProject-2.1.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.pom
Download https://repo1.maven.org/maven2/org/apache/logging/log4j/log4j-api/2.1/log4j-api-2.1.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.pom
Download https://repo1.maven.org/maven2/tomcat/servlet-api/5.5.23/servlet-api-5.5.23.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-project-dist/2.2.0/hadoop-project-dist-2.2.0.pom
Download https://repo1.maven.org/maven2/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.pom
Download https://repo1.maven.org/maven2/com/codepoetics/protonpack/1.1/protonpack-1.1.pom
Download https://repo1.maven.org/maven2/net/sf/opencsv/opencsv/2.3/opencsv-2.3.pom
Download https://repo1.maven.org/maven2/org/ow2/asm/asm-all/4.1/asm-all-4.1.pom
Download https://repo1.maven.org/maven2/commons-configuration/commons-configuration/1.7/commons-configuration-1.7.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-mapreduce-client/2.2.0/hadoop-mapreduce-client-2.2.0.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-project/2.2.0/hadoop-project-2.2.0.pom
Download https://repo1.maven.org/maven2/tomcat/tomcat-parent/5.5.23/tomcat-parent-5.5.23.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-main/2.2.0/hadoop-main-2.2.0.pom
Download https://repo1.maven.org/maven2/org/apache/directory/studio/org.apache.commons.codec/1.8/org.apache.commons.codec-1.8.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-jackson/0.8.0/nd4j-jackson-0.8.0.pom
Download https://repo1.maven.org/maven2/org/deeplearning4j/deeplearning4j-core/0.8.0/deeplearning4j-core-0.8.0.pom
Download https://repo1.maven.org/maven2/org/apache/directory/studio/parent-libraries/2.0.0.v20130628/parent-libraries-2.0.0.v20130628.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-native-api/0.8.0/nd4j-native-api-0.8.0.pom
Download https://repo1.maven.org/maven2/org/apache/directory/studio/parent/2.0.0.v20130628/parent-2.0.0.v20130628.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-serde/0.8.0/nd4j-serde-0.8.0.pom
Download https://repo1.maven.org/maven2/org/apache/directory/project/project/31/project-31.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-api-parent/0.8.0/nd4j-api-parent-0.8.0.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-native/0.8.0/nd4j-native-0.8.0.pom
Download https://repo1.maven.org/maven2/xalan/xalan/2.7.0/xalan-2.7.0.pom
Download https://repo1.maven.org/maven2/xerces/xercesImpl/2.8.0/xercesImpl-2.8.0.pom
Download https://repo1.maven.org/maven2/javax/xml/bind/jaxb-api/2.2.7/jaxb-api-2.2.7.pom
Download https://repo1.maven.org/maven2/commons-el/commons-el/1.0/commons-el-1.0.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.pom
Download https://repo1.maven.org/maven2/xmlenc/xmlenc/0.52/xmlenc-0.52.pom
Download https://repo1.maven.org/maven2/org/apache/commons/commons-math/2.1/commons-math-2.1.pom
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-core/1.9/jersey-core-1.9.pom
Download https://repo1.maven.org/maven2/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.pom
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-server/1.9/jersey-server-1.9.pom
Download https://repo1.maven.org/maven2/net/java/dev/jets3t/jets3t/0.6.1/jets3t-0.6.1.pom
Download https://repo1.maven.org/maven2/commons-net/commons-net/3.1/commons-net-3.1.pom
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-json/1.9/jersey-json-1.9.pom
Download https://repo1.maven.org/maven2/org/apache/avro/avro/1.7.4/avro-1.7.4.pom
Download https://repo1.maven.org/maven2/tomcat/jasper-compiler/5.5.23/jasper-compiler-5.5.23.pom
Download https://repo1.maven.org/maven2/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.pom
Download https://repo1.maven.org/maven2/org/mortbay/jetty/jetty/6.1.26/jetty-6.1.26.pom
Download https://repo1.maven.org/maven2/tomcat/jasper-runtime/5.5.23/jasper-runtime-5.5.23.pom
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-project/1.9/jersey-project-1.9.pom
Download https://repo1.maven.org/maven2/com/jcraft/jsch/0.1.42/jsch-0.1.42.pom
Download https://repo1.maven.org/maven2/org/apache/avro/avro-parent/1.7.4/avro-parent-1.7.4.pom
Download https://repo1.maven.org/maven2/org/mortbay/jetty/project/6.1.26/project-6.1.26.pom
Download https://repo1.maven.org/maven2/org/apache/avro/avro-toplevel/1.7.4/avro-toplevel-1.7.4.pom
Download https://repo1.maven.org/maven2/commons-daemon/commons-daemon/1.0.13/commons-daemon-1.0.13.pom
Download https://repo1.maven.org/maven2/com/google/inject/extensions/guice-servlet/3.0/guice-servlet-3.0.pom
Download https://repo1.maven.org/maven2/io/netty/netty/3.6.2.Final/netty-3.6.2.Final.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.pom
Download https://repo1.maven.org/maven2/com/google/inject/extensions/extensions-parent/3.0/extensions-parent-3.0.pom
Download https://repo1.maven.org/maven2/com/google/inject/guice-parent/3.0/guice-parent-3.0.pom
Download https://repo1.maven.org/maven2/jline/jline/0.9.94/jline-0.9.94.pom
Download https://repo1.maven.org/maven2/org/jboss/netty/netty/3.2.2.Final/netty-3.2.2.Final.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp/1.3.2/javacpp-1.3.2.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-buffer/0.8.0/nd4j-buffer-0.8.0.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-api/0.8.0/nd4j-api-0.8.0.pom
Download https://repo1.maven.org/maven2/org/json/json/20131018/json-20131018.pom
Download https://repo1.maven.org/maven2/org/projectlombok/lombok/1.16.10/lombok-1.16.10.pom
Download https://repo1.maven.org/maven2/org/datavec/datavec-data-image/0.8.0/datavec-data-image-0.8.0.pom
Download https://repo1.maven.org/maven2/org/datavec/datavec-api/0.8.0/datavec-api-0.8.0.pom
Download https://repo1.maven.org/maven2/org/deeplearning4j/deeplearning4j-nn/0.8.0/deeplearning4j-nn-0.8.0.pom
Download https://repo1.maven.org/maven2/org/deeplearning4j/deeplearning4j-modelimport/0.8.0/deeplearning4j-modelimport-0.8.0.pom
Download https://repo1.maven.org/maven2/org/nd4j/jackson/0.8.0/jackson-0.8.0.pom
Download https://repo1.maven.org/maven2/org/deeplearning4j/deeplearning4j-ui-components/0.8.0/deeplearning4j-ui-components-0.8.0.pom
Download https://repo1.maven.org/maven2/org/datavec/datavec-nd4j-common/0.8.0/datavec-nd4j-common-0.8.0.pom
Download https://repo1.maven.org/maven2/org/datavec/datavec-parent/0.8.0/datavec-parent-0.8.0.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-shade/0.8.0/nd4j-shade-0.8.0.pom
Download https://repo1.maven.org/maven2/org/datavec/datavec-data/0.8.0/datavec-data-0.8.0.pom
Download https://repo1.maven.org/maven2/org/deeplearning4j/deeplearning4j-ui-parent/0.8.0/deeplearning4j-ui-parent-0.8.0.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-base64/0.8.0/nd4j-base64-0.8.0.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/openblas-platform/0.2.19-1.3/openblas-platform-0.2.19-1.3.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/1.3/javacpp-presets-1.3.pom
Download https://repo1.maven.org/maven2/com/sun/xml/bind/jaxb-impl/2.2.3-1/jaxb-impl-2.2.3-1.pom
Download https://repo1.maven.org/maven2/org/codehaus/jettison/jettison/1.1/jettison-1.1.pom
Download https://repo1.maven.org/maven2/org/codehaus/jackson/jackson-xc/1.8.3/jackson-xc-1.8.3.pom
Download https://repo1.maven.org/maven2/org/codehaus/jackson/jackson-jaxrs/1.8.3/jackson-jaxrs-1.8.3.pom
Download https://repo1.maven.org/maven2/asm/asm/3.1/asm-3.1.pom
Download https://repo1.maven.org/maven2/asm/asm-parent/3.1/asm-parent-3.1.pom
Download https://repo1.maven.org/maven2/com/thoughtworks/paranamer/paranamer/2.3/paranamer-2.3.pom
Download https://repo1.maven.org/maven2/org/xerial/snappy/snappy-java/1.0.4.1/snappy-java-1.0.4.1.pom
Download https://repo1.maven.org/maven2/com/thoughtworks/paranamer/paranamer-parent/2.3/paranamer-parent-2.3.pom
Download https://repo1.maven.org/maven2/org/codehaus/codehaus-parent/1/codehaus-parent-1.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-yarn-server/2.2.0/hadoop-yarn-server-2.2.0.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-yarn/2.2.0/hadoop-yarn-2.2.0.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-yarn-server-nodemanager/2.2.0/hadoop-yarn-server-nodemanager-2.2.0.pom
Download https://repo1.maven.org/maven2/com/google/inject/guice/3.0/guice-3.0.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-context/0.8.0/nd4j-context-0.8.0.pom
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-common/0.8.0/nd4j-common-0.8.0.pom
Download https://repo1.maven.org/maven2/net/ericaro/neoitertools/1.0.0/neoitertools-1.0.0.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/hdf5-platform/1.10.0-patch1-1.3/hdf5-platform-1.10.0-patch1-1.3.pom
Download https://repo1.maven.org/maven2/org/yaml/snakeyaml/1.12/snakeyaml-1.12.pom
Download https://repo1.maven.org/maven2/org/freemarker/freemarker/2.3.23/freemarker-2.3.23.pom
Download https://repo1.maven.org/maven2/com/clearspring/analytics/stream/2.7.0/stream-2.7.0.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/opencv-platform/3.1.0-1.3/opencv-platform-3.1.0-1.3.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacv/1.3.1/javacv-1.3.1.pom
Download https://repo1.maven.org/maven2/com/twelvemonkeys/imageio/imageio-psd/3.1.1/imageio-psd-3.1.1.pom
Download https://repo1.maven.org/maven2/com/twelvemonkeys/imageio/imageio-tiff/3.1.1/imageio-tiff-3.1.1.pom
Download https://repo1.maven.org/maven2/com/twelvemonkeys/imageio/imageio-jpeg/3.1.1/imageio-jpeg-3.1.1.pom
Download https://repo1.maven.org/maven2/com/twelvemonkeys/imageio/imageio-bmp/3.1.1/imageio-bmp-3.1.1.pom
Download https://repo1.maven.org/maven2/com/github/jai-imageio/jai-imageio-core/1.3.0/jai-imageio-core-1.3.0.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/leptonica-platform/1.73-1.3/leptonica-platform-1.73-1.3.pom
Download https://repo1.maven.org/maven2/com/twelvemonkeys/imageio/imageio/3.1.1/imageio-3.1.1.pom
Download https://repo1.maven.org/maven2/com/twelvemonkeys/twelvemonkeys/3.1.1/twelvemonkeys-3.1.1.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/openblas/0.2.19-1.3/openblas-0.2.19-1.3.pom
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.pom
Download https://repo1.maven.org/maven2/com/sun/jersey/contribs/jersey-guice/1.9/jersey-guice-1.9.pom
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-test-framework/jersey-test-framework-grizzly2/1.9/jersey-test-framework-grizzly2-1.9.pom
Download https://repo1.maven.org/maven2/com/sun/jersey/contribs/jersey-contribs/1.9/jersey-contribs-1.9.pom
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-test-framework/1.9/jersey-test-framework-1.9.pom
Download https://repo1.maven.org/maven2/org/sonatype/sisu/inject/cglib/2.2.1-v20090111/cglib-2.2.1-v20090111.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/hdf5/1.10.0-patch1-1.3/hdf5-1.10.0-patch1-1.3.pom
Download https://repo1.maven.org/maven2/org/javassist/javassist/3.18.2-GA/javassist-3.18.2-GA.pom
Download https://repo1.maven.org/maven2/it/unimi/dsi/fastutil/6.5.7/fastutil-6.5.7.pom
Download https://repo1.maven.org/maven2/com/twelvemonkeys/common/common-lang/3.1.1/common-lang-3.1.1.pom
Download https://repo1.maven.org/maven2/com/twelvemonkeys/imageio/imageio-core/3.1.1/imageio-core-3.1.1.pom
Download https://repo1.maven.org/maven2/com/twelvemonkeys/imageio/imageio-metadata/3.1.1/imageio-metadata-3.1.1.pom
Download https://repo1.maven.org/maven2/com/twelvemonkeys/common/common-io/3.1.1/common-io-3.1.1.pom
Download https://repo1.maven.org/maven2/com/twelvemonkeys/common/common/3.1.1/common-3.1.1.pom
Download https://repo1.maven.org/maven2/com/twelvemonkeys/common/common-image/3.1.1/common-image-3.1.1.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/flycapture/2.9.3.43-1.3/flycapture-2.9.3.43-1.3.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/videoinput/0.200-1.3/videoinput-0.200-1.3.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/ffmpeg/3.2.1-1.3/ffmpeg-3.2.1-1.3.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/opencv/3.1.0-1.3/opencv-3.1.0-1.3.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/libfreenect2/0.2.0-1.3/libfreenect2-0.2.0-1.3.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/libdc1394/2.2.4-1.3/libdc1394-2.2.4-1.3.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/libfreenect/0.5.3-1.3/libfreenect-0.5.3-1.3.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/librealsense/1.9.6-1.3/librealsense-1.9.6-1.3.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/artoolkitplus/2.3.1-1.3/artoolkitplus-2.3.1-1.3.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/flandmark/1.07-1.3/flandmark-1.07-1.3.pom
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/leptonica/1.73-1.3/leptonica-1.73-1.3.pom
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-grizzly2/1.9/jersey-grizzly2-1.9.pom
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-test-framework/jersey-test-framework-core/1.9/jersey-test-framework-core-1.9.pom
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-client/1.9/jersey-client-1.9.pom
Download https://repo1.maven.org/maven2/org/glassfish/grizzly/grizzly-http-servlet/2.1.2/grizzly-http-servlet-2.1.2.pom
Download https://repo1.maven.org/maven2/org/glassfish/grizzly/grizzly-http/2.1.2/grizzly-http-2.1.2.pom
Download https://repo1.maven.org/maven2/org/glassfish/javax.servlet/3.1/javax.servlet-3.1.pom
Download https://repo1.maven.org/maven2/org/glassfish/grizzly/grizzly-http-server/2.1.2/grizzly-http-server-2.1.2.pom
Download https://repo1.maven.org/maven2/org/glassfish/grizzly/grizzly-project/2.1.2/grizzly-project-2.1.2.pom
Download https://repo1.maven.org/maven2/org/glassfish/api-pom/3.1/api-pom-3.1.pom
Download https://repo1.maven.org/maven2/org/glassfish/glassfish-parent/3.1/glassfish-parent-3.1.pom
Download https://repo1.maven.org/maven2/org/glassfish/grizzly/grizzly-framework/2.1.2/grizzly-framework-2.1.2.pom
Download https://repo1.maven.org/maven2/org/glassfish/grizzly/grizzly-rcm/2.1.2/grizzly-rcm-2.1.2.pom
Download https://repo1.maven.org/maven2/org/glassfish/gmbal/gmbal-api-only/3.0.0-b023/gmbal-api-only-3.0.0-b023.pom
Download https://repo1.maven.org/maven2/org/glassfish/external/management-api/3.0.0-b012/management-api-3.0.0-b012.pom
Download https://repo1.maven.org/maven2/commons-digester/commons-digester/1.8.1/commons-digester-1.8.1.pom
Download https://repo1.maven.org/maven2/org/apache/commons/commons-math3/3.4.1/commons-math3-3.4.1.pom
Download https://repo1.maven.org/maven2/org/apache/commons/commons-compress/1.8.1/commons-compress-1.8.1.pom

> Task :compileKotlin 
POM relocation to an other version number is not fully supported in Gradle : xml-apis:xml-apis:2.0.2 relocated to xml-apis:xml-apis:1.0.b2.
Please update your dependency to directly use the correct version 'xml-apis:xml-apis:1.0.b2'.
Resolution will only pick dependencies of the relocated element.  Artifacts and other metadata will be ignored.

Download https://repo1.maven.org/maven2/edu/stanford/nlp/stanford-corenlp/3.6.0/stanford-corenlp-3.6.0.jar
Download https://repo1.maven.org/maven2/com/beust/jcommander/1.69/jcommander-1.69.jar
Download https://repo1.maven.org/maven2/de/jungblut/jrpt/jrpt/0.1/jrpt-0.1.jar
Download https://repo1.maven.org/maven2/com/github/javaparser/javaparser-core/3.5.4/javaparser-core-3.5.4.jar
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-hdfs/2.2.0/hadoop-hdfs-2.2.0.jar
Download https://repo1.maven.org/maven2/org/jsoup/jsoup/1.8.3/jsoup-1.8.3.jar
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-common/2.2.0/hadoop-common-2.2.0.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-native-platform/0.8.0/nd4j-native-platform-0.8.0.jar
Download https://repo1.maven.org/maven2/org/deeplearning4j/deeplearning4j-nlp/0.8.0/deeplearning4j-nlp-0.8.0.jar
Download https://repo1.maven.org/maven2/org/datavec/datavec-nd4j-common/0.8.0/datavec-nd4j-common-0.8.0.jar
Download https://repo1.maven.org/maven2/de/jungblut/common/thomasjungblut-common/1.1/thomasjungblut-common-1.1.jar
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-mapreduce-client-common/2.2.0/hadoop-mapreduce-client-common-2.2.0.jar
Download https://repo1.maven.org/maven2/org/datavec/datavec-api/0.8.0/datavec-api-0.8.0.jar
Download https://repo1.maven.org/maven2/org/deeplearning4j/deeplearning4j-modelimport/0.8.0/deeplearning4j-modelimport-0.8.0.jar
Download https://repo1.maven.org/maven2/org/datavec/datavec-data-image/0.8.0/datavec-data-image-0.8.0.jar
Download https://repo1.maven.org/maven2/de/jungblut/math/tjungblut-math/1.3/tjungblut-math-1.3.jar
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-mapreduce-client-jobclient/2.2.0/hadoop-mapreduce-client-jobclient-2.2.0.jar
Download https://repo1.maven.org/maven2/org/deeplearning4j/deeplearning4j-core/0.8.0/deeplearning4j-core-0.8.0.jar
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-mapreduce-client-shuffle/2.2.0/hadoop-mapreduce-client-shuffle-2.2.0.jar
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-yarn-client/2.2.0/hadoop-yarn-client-2.2.0.jar
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-yarn-server-common/2.2.0/hadoop-yarn-server-common-2.2.0.jar
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-mapreduce-client-core/2.2.0/hadoop-mapreduce-client-core-2.2.0.jar
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-yarn-server-nodemanager/2.2.0/hadoop-yarn-server-nodemanager-2.2.0.jar
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-yarn-common/2.2.0/hadoop-yarn-common-2.2.0.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-native/0.8.0/nd4j-native-0.8.0.jar
Download https://repo1.maven.org/maven2/edu/stanford/nlp/stanford-corenlp/3.6.0/stanford-corenlp-3.6.0-models-english.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-native/0.8.0/nd4j-native-0.8.0-linux-x86_64.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-base64/0.8.0/nd4j-base64-0.8.0.jar
Download https://repo1.maven.org/maven2/org/deeplearning4j/deeplearning4j-ui-components/0.8.0/deeplearning4j-ui-components-0.8.0.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-native-api/0.8.0/nd4j-native-api-0.8.0.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-jackson/0.8.0/nd4j-jackson-0.8.0.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-native/0.8.0/nd4j-native-0.8.0-macosx-x86_64.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-native/0.8.0/nd4j-native-0.8.0-linux-ppc64le.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-api/0.8.0/nd4j-api-0.8.0.jar
Download https://repo1.maven.org/maven2/org/slf4j/slf4j-simple/1.7.21/slf4j-simple-1.7.21.jar
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-yarn-api/2.2.0/hadoop-yarn-api-2.2.0.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-native/0.8.0/nd4j-native-0.8.0-android-x86.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-buffer/0.8.0/nd4j-buffer-0.8.0.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-context/0.8.0/nd4j-context-0.8.0.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-common/0.8.0/nd4j-common-0.8.0.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-native/0.8.0/nd4j-native-0.8.0-windows-x86_64.jar
Download https://repo1.maven.org/maven2/de/jollyday/jollyday/0.4.7/jollyday-0.4.7.jar
Download https://repo1.maven.org/maven2/org/nd4j/nd4j-native/0.8.0/nd4j-native-0.8.0-android-arm.jar
Download https://repo1.maven.org/maven2/org/apache/zookeeper/zookeeper/3.4.5/zookeeper-3.4.5.jar
Download https://repo1.maven.org/maven2/com/io7m/xom/xom/1.2.10/xom-1.2.10.jar
Download https://repo1.maven.org/maven2/com/googlecode/efficient-java-matrix-library/ejml/0.23/ejml-0.23.jar
Download https://repo1.maven.org/maven2/javax/json/javax.json-api/1.0/javax.json-api-1.0.jar
Download https://repo1.maven.org/maven2/org/apache/avro/avro/1.7.4/avro-1.7.4.jar
Download https://repo1.maven.org/maven2/org/nd4j/jackson/0.8.0/jackson-0.8.0.jar
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-auth/2.2.0/hadoop-auth-2.2.0.jar
Download https://repo1.maven.org/maven2/org/mdkt/compiler/InMemoryJavaCompiler/1.3.0/InMemoryJavaCompiler-1.3.0.jar
Download https://repo1.maven.org/maven2/org/apache/commons/commons-math3/3.4.1/commons-math3-3.4.1.jar
Download https://repo1.maven.org/maven2/jline/jline/0.9.94/jline-0.9.94.jar
Download https://repo1.maven.org/maven2/net/ericaro/neoitertools/1.0.0/neoitertools-1.0.0.jar
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-test-framework/jersey-test-framework-grizzly2/1.9/jersey-test-framework-grizzly2-1.9.jar
Download https://repo1.maven.org/maven2/net/sf/trove4j/trove4j/3.0.2/trove4j-3.0.2.jar
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-test-framework/jersey-test-framework-core/1.9/jersey-test-framework-core-1.9.jar
Download https://repo1.maven.org/maven2/org/htmlparser/htmllexer/2.1/htmllexer-2.1.jar
Download https://repo1.maven.org/maven2/net/sf/opencsv/opencsv/2.3/opencsv-2.3.jar
Download https://repo1.maven.org/maven2/net/java/dev/jets3t/jets3t/0.6.1/jets3t-0.6.1.jar
Download https://repo1.maven.org/maven2/net/sourceforge/nekohtml/nekohtml/1.9.17/nekohtml-1.9.17.jar
Download https://repo1.maven.org/maven2/org/codehaus/jackson/jackson-jaxrs/1.8.3/jackson-jaxrs-1.8.3.jar
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-json/1.9/jersey-json-1.9.jar
Download https://repo1.maven.org/maven2/org/codehaus/jackson/jackson-xc/1.8.3/jackson-xc-1.8.3.jar
Download https://repo1.maven.org/maven2/org/htmlparser/htmlparser/2.1/htmlparser-2.1.jar
Download https://repo1.maven.org/maven2/com/codepoetics/protonpack/1.1/protonpack-1.1.jar
Download https://repo1.maven.org/maven2/org/codehaus/jackson/jackson-core-asl/1.9.11/jackson-core-asl-1.9.11.jar
Download https://repo1.maven.org/maven2/org/codehaus/jackson/jackson-mapper-asl/1.9.11/jackson-mapper-asl-1.9.11.jar
Download https://repo1.maven.org/maven2/commons-digester/commons-digester/1.8.1/commons-digester-1.8.1.jar
Download https://repo1.maven.org/maven2/org/apache/logging/log4j/log4j-api/2.1/log4j-api-2.1.jar
Download https://repo1.maven.org/maven2/commons-el/commons-el/1.0/commons-el-1.0.jar
Download https://repo1.maven.org/maven2/commons-beanutils/commons-beanutils/1.8.3/commons-beanutils-1.8.3.jar
Download https://repo1.maven.org/maven2/org/mockito/mockito-all/1.9.5/mockito-all-1.9.5.jar
Download https://repo1.maven.org/maven2/org/apache/mrunit/mrunit/1.0.0/mrunit-1.0.0-hadoop2.jar
Download https://repo1.maven.org/maven2/org/ow2/asm/asm-all/4.1/asm-all-4.1.jar
Download https://repo1.maven.org/maven2/tomcat/jasper-runtime/5.5.23/jasper-runtime-5.5.23.jar
Download https://repo1.maven.org/maven2/de/l3s/boilerpipe/boilerpipe/1.1.0/boilerpipe-1.1.0.jar
Download https://repo1.maven.org/maven2/xalan/xalan/2.7.0/xalan-2.7.0.jar
Download https://repo1.maven.org/maven2/com/sun/xml/bind/jaxb-impl/2.2.3-1/jaxb-impl-2.2.3-1.jar
Download https://repo1.maven.org/maven2/org/apache/commons/commons-math/2.1/commons-math-2.1.jar
Download https://repo1.maven.org/maven2/org/apache/directory/studio/org.apache.commons.codec/1.8/org.apache.commons.codec-1.8.jar
Download https://repo1.maven.org/maven2/javax/xml/bind/jaxb-api/2.2.7/jaxb-api-2.2.7.jar
Download https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-annotations/2.2.0/hadoop-annotations-2.2.0.jar
Download https://repo1.maven.org/maven2/tomcat/servlet-api/5.5.23/servlet-api-5.5.23.jar
Download https://repo1.maven.org/maven2/commons-configuration/commons-configuration/1.7/commons-configuration-1.7.jar
Download https://repo1.maven.org/maven2/xmlenc/xmlenc/0.52/xmlenc-0.52.jar
Download https://repo1.maven.org/maven2/org/apache/logging/log4j/log4j-core/2.1/log4j-core-2.1.jar
Download https://repo1.maven.org/maven2/org/mortbay/jetty/jetty-util/6.1.26/jetty-util-6.1.26.jar
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-server/1.9/jersey-server-1.9.jar
Download https://repo1.maven.org/maven2/org/mortbay/jetty/jetty/6.1.26/jetty-6.1.26.jar
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-grizzly2/1.9/jersey-grizzly2-1.9.jar
Download https://repo1.maven.org/maven2/tomcat/jasper-compiler/5.5.23/jasper-compiler-5.5.23.jar
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-client/1.9/jersey-client-1.9.jar
Download https://repo1.maven.org/maven2/commons-net/commons-net/3.1/commons-net-3.1.jar
Download https://repo1.maven.org/maven2/com/google/protobuf/protobuf-java/2.5.0/protobuf-java-2.5.0.jar
Download https://repo1.maven.org/maven2/org/apache/commons/commons-compress/1.8.1/commons-compress-1.8.1.jar
Download https://repo1.maven.org/maven2/com/sun/jersey/contribs/jersey-guice/1.9/jersey-guice-1.9.jar
Download https://repo1.maven.org/maven2/com/sun/jersey/jersey-core/1.9/jersey-core-1.9.jar
Download https://repo1.maven.org/maven2/commons-daemon/commons-daemon/1.0.13/commons-daemon-1.0.13.jar
Download https://repo1.maven.org/maven2/com/jcraft/jsch/0.1.42/jsch-0.1.42.jar
Download https://repo1.maven.org/maven2/io/netty/netty/3.6.2.Final/netty-3.6.2.Final.jar
Download https://repo1.maven.org/maven2/com/google/inject/extensions/guice-servlet/3.0/guice-servlet-3.0.jar
Download https://repo1.maven.org/maven2/org/jboss/netty/netty/3.2.2.Final/netty-3.2.2.Final.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/openblas-platform/0.2.19-1.3/openblas-platform-0.2.19-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacv/1.3.1/javacv-1.3.1.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/openblas/0.2.19-1.3/openblas-0.2.19-1.3-linux-x86.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/openblas/0.2.19-1.3/openblas-0.2.19-1.3-windows-x86_64.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/openblas/0.2.19-1.3/openblas-0.2.19-1.3-android-x86.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/hdf5/1.10.0-patch1-1.3/hdf5-1.10.0-patch1-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/openblas/0.2.19-1.3/openblas-0.2.19-1.3-windows-x86.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/openblas/0.2.19-1.3/openblas-0.2.19-1.3-macosx-x86_64.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/openblas/0.2.19-1.3/openblas-0.2.19-1.3-linux-x86_64.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/hdf5-platform/1.10.0-patch1-1.3/hdf5-platform-1.10.0-patch1-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/openblas/0.2.19-1.3/openblas-0.2.19-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/openblas/0.2.19-1.3/openblas-0.2.19-1.3-linux-ppc64le.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/openblas/0.2.19-1.3/openblas-0.2.19-1.3-linux-armhf.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/hdf5/1.10.0-patch1-1.3/hdf5-1.10.0-patch1-1.3-macosx-x86_64.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/openblas/0.2.19-1.3/openblas-0.2.19-1.3-android-arm.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/hdf5/1.10.0-patch1-1.3/hdf5-1.10.0-patch1-1.3-windows-x86.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/hdf5/1.10.0-patch1-1.3/hdf5-1.10.0-patch1-1.3-linux-x86.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/hdf5/1.10.0-patch1-1.3/hdf5-1.10.0-patch1-1.3-linux-ppc64le.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/hdf5/1.10.0-patch1-1.3/hdf5-1.10.0-patch1-1.3-windows-x86_64.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/opencv-platform/3.1.0-1.3/opencv-platform-3.1.0-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/hdf5/1.10.0-patch1-1.3/hdf5-1.10.0-patch1-1.3-linux-x86_64.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/flandmark/1.07-1.3/flandmark-1.07-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/opencv/3.1.0-1.3/opencv-3.1.0-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/opencv/3.1.0-1.3/opencv-3.1.0-1.3-android-arm.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/opencv/3.1.0-1.3/opencv-3.1.0-1.3-linux-x86.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/opencv/3.1.0-1.3/opencv-3.1.0-1.3-android-x86.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/opencv/3.1.0-1.3/opencv-3.1.0-1.3-linux-x86_64.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/opencv/3.1.0-1.3/opencv-3.1.0-1.3-linux-armhf.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/ffmpeg/3.2.1-1.3/ffmpeg-3.2.1-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/opencv/3.1.0-1.3/opencv-3.1.0-1.3-windows-x86_64.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/flycapture/2.9.3.43-1.3/flycapture-2.9.3.43-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/opencv/3.1.0-1.3/opencv-3.1.0-1.3-linux-ppc64le.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/opencv/3.1.0-1.3/opencv-3.1.0-1.3-windows-x86.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/opencv/3.1.0-1.3/opencv-3.1.0-1.3-macosx-x86_64.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/libfreenect2/0.2.0-1.3/libfreenect2-0.2.0-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/libfreenect/0.5.3-1.3/libfreenect-0.5.3-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/libdc1394/2.2.4-1.3/libdc1394-2.2.4-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/leptonica/1.73-1.3/leptonica-1.73-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/leptonica-platform/1.73-1.3/leptonica-platform-1.73-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/videoinput/0.200-1.3/videoinput-0.200-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/leptonica/1.73-1.3/leptonica-1.73-1.3-linux-x86.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/artoolkitplus/2.3.1-1.3/artoolkitplus-2.3.1-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/librealsense/1.9.6-1.3/librealsense-1.9.6-1.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/leptonica/1.73-1.3/leptonica-1.73-1.3-android-arm.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/leptonica/1.73-1.3/leptonica-1.73-1.3-android-x86.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/leptonica/1.73-1.3/leptonica-1.73-1.3-windows-x86.jar
Download https://repo1.maven.org/maven2/org/projectlombok/lombok/1.16.10/lombok-1.16.10.jar
Download https://repo1.maven.org/maven2/com/google/inject/guice/3.0/guice-3.0.jar
Download https://repo1.maven.org/maven2/org/json/json/20131018/json-20131018.jar
Download https://repo1.maven.org/maven2/org/codehaus/jettison/jettison/1.1/jettison-1.1.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/leptonica/1.73-1.3/leptonica-1.73-1.3-macosx-x86_64.jar
Download https://repo1.maven.org/maven2/asm/asm/3.1/asm-3.1.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp/1.3.2/javacpp-1.3.2.jar
Download https://repo1.maven.org/maven2/org/sonatype/sisu/inject/cglib/2.2.1-v20090111/cglib-2.2.1-v20090111.jar
Download https://repo1.maven.org/maven2/com/thoughtworks/paranamer/paranamer/2.3/paranamer-2.3.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/leptonica/1.73-1.3/leptonica-1.73-1.3-windows-x86_64.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/leptonica/1.73-1.3/leptonica-1.73-1.3-linux-x86_64.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/leptonica/1.73-1.3/leptonica-1.73-1.3-linux-armhf.jar
Download https://repo1.maven.org/maven2/org/xerial/snappy/snappy-java/1.0.4.1/snappy-java-1.0.4.1.jar
Download https://repo1.maven.org/maven2/org/yaml/snakeyaml/1.12/snakeyaml-1.12.jar
Download https://repo1.maven.org/maven2/org/freemarker/freemarker/2.3.23/freemarker-2.3.23.jar
Download https://repo1.maven.org/maven2/com/twelvemonkeys/imageio/imageio-jpeg/3.1.1/imageio-jpeg-3.1.1.jar
Download https://repo1.maven.org/maven2/com/twelvemonkeys/imageio/imageio-tiff/3.1.1/imageio-tiff-3.1.1.jar
Download https://repo1.maven.org/maven2/com/twelvemonkeys/imageio/imageio-psd/3.1.1/imageio-psd-3.1.1.jar
Download https://repo1.maven.org/maven2/com/github/jai-imageio/jai-imageio-core/1.3.0/jai-imageio-core-1.3.0.jar
Download https://repo1.maven.org/maven2/org/bytedeco/javacpp-presets/leptonica/1.73-1.3/leptonica-1.73-1.3-linux-ppc64le.jar
Download https://repo1.maven.org/maven2/com/twelvemonkeys/imageio/imageio-bmp/3.1.1/imageio-bmp-3.1.1.jar
Download https://repo1.maven.org/maven2/com/clearspring/analytics/stream/2.7.0/stream-2.7.0.jar
Download https://repo1.maven.org/maven2/org/javassist/javassist/3.18.2-GA/javassist-3.18.2-GA.jar
Download https://repo1.maven.org/maven2/com/twelvemonkeys/imageio/imageio-core/3.1.1/imageio-core-3.1.1.jar
Download https://repo1.maven.org/maven2/com/twelvemonkeys/common/common-io/3.1.1/common-io-3.1.1.jar
Download https://repo1.maven.org/maven2/org/glassfish/grizzly/grizzly-http-servlet/2.1.2/grizzly-http-servlet-2.1.2.jar
Download https://repo1.maven.org/maven2/it/unimi/dsi/fastutil/6.5.7/fastutil-6.5.7.jar
Download https://repo1.maven.org/maven2/com/twelvemonkeys/imageio/imageio-metadata/3.1.1/imageio-metadata-3.1.1.jar
Download https://repo1.maven.org/maven2/org/glassfish/grizzly/grizzly-http/2.1.2/grizzly-http-2.1.2.jar
Download https://repo1.maven.org/maven2/org/glassfish/external/management-api/3.0.0-b012/management-api-3.0.0-b012.jar
Download https://repo1.maven.org/maven2/org/glassfish/grizzly/grizzly-http-server/2.1.2/grizzly-http-server-2.1.2.jar
Download https://repo1.maven.org/maven2/org/glassfish/gmbal/gmbal-api-only/3.0.0-b023/gmbal-api-only-3.0.0-b023.jar
Download https://repo1.maven.org/maven2/org/glassfish/javax.servlet/3.1/javax.servlet-3.1.jar
Download https://repo1.maven.org/maven2/com/twelvemonkeys/common/common-lang/3.1.1/common-lang-3.1.1.jar
Download https://repo1.maven.org/maven2/org/glassfish/grizzly/grizzly-rcm/2.1.2/grizzly-rcm-2.1.2.jar
Download https://repo1.maven.org/maven2/com/twelvemonkeys/common/common-image/3.1.1/common-image-3.1.1.jar
Download https://repo1.maven.org/maven2/org/glassfish/grizzly/grizzly-framework/2.1.2/grizzly-framework-2.1.2.jar
Download https://repo1.maven.org/maven2/org/deeplearning4j/deeplearning4j-nn/0.8.0/deeplearning4j-nn-0.8.0.jar

> Task :compileJava 
/home/auri/OneDrive/temp/00-orientacoes/andre-pestana/workspace/toradocu/src/main/java/org/toradocu/translator/semantic/GloveModelWrapper.java:54: warning: [deprecation] loadTxtVectors(File) in WordVectorSerializer has been deprecated
      gloveVectors = WordVectorSerializer.loadTxtVectors(gloveFinalFile);
                                         ^
1 warning

Download http://star-rep.inf.usi.ch/alberto/glove/raw/master/glove-binary.zip
Download http://star-rep.inf.usi.ch/alberto/glove/raw/master/glove-models.zip

BUILD SUCCESSFUL in 12m 42s
8 actionable tasks: 8 executed
auri@av01:~/OneDrive/temp/00-orientacoes/andre-pestana/workspace/toradocu$ 
```

## Tutorial

Download `.jar` dependencies:

(`junit-4.12.jar`)[https://mvnrepository.com/artifact/junit/junit/4.12]

(`hamcrest-core-1.3.jar`)[https://mvnrepository.com/artifact/org.hamcrest/hamcrest-core/1.3]

(`aspectjrt-1.8.9.jar`)[https://mvnrepository.com/artifact/org.aspectj/aspectjrt/1.8.9]

(`aspectjtools-1.8.9.jar`)[https://mvnrepository.com/artifact/org.aspectj/aspectjtools/1.8.9]

(`aspectjweaver-1.8.9.jar`)[https://mvnrepository.com/artifact/org.aspectj/aspectjweaver/1.8.9]

Save jar files inside `tutorial/lib` directory

```shell
cd tutorial
mkdir lib
```

```
tutorial/
├── lib
│   ├── hamcrest-core-1.3.jar
│   └── junit-4.12.jar
├── README.md
├── src
│   └── net
│       ├── Connection.class
│       └── Connection.java
└── test
    └── net
        ├── ConnectionTest.class
        └── ConnectionTest.java

6 directories, 7 files

```


Compile tutorial classes:

```shell
javac src/net/Connection.java
```


Compile tutorial test set:
```shell
javac -cp lib/junit-4.12.jar:src test/net/ConnectionTest.java
```

Final directory structure:

```
tutorial/
├── lib
│   ├── hamcrest-core-1.3.jar
│   └── junit-4.12.jar
├── README.md
├── src
│   └── net
│       ├── Connection.class
│       └── Connection.java
└── test
    └── net
        ├── ConnectionTest.class
        └── ConnectionTest.java

6 directories, 7 files

```

Run test set:


```shell
java -cp lib/junit-4.12.jar:lib/hamcrest-core-1.3.jar:test:src org.junit.runner.JUnitCore net.ConnectionTest
```


Teste execution output as expected:

```JUnit version 4.12
..E
Time: 0,007
There was 1 failure:
1) send(net.ConnectionTest)
java.lang.NullPointerException
	at net.Connection.send(Connection.java:33)
	at net.ConnectionTest.send(ConnectionTest.java:20)
	...
	at org.junit.runner.JUnitCore.runMain(JUnitCore.java:77)
	at org.junit.runner.JUnitCore.main(JUnitCore.java:36)

FAILURES!!!
Tests run: 2,  Failures: 1

```

## Run Toradoc


```shell
java -jar ../build/libs/toradocu-1.0-all.jar \
--target-class net.Connection \
--test-class net.ConnectionTest \
--source-dir src \
--class-dir src \
--aspects-output-dir aspects \
--oracle-generation true

```

Tool output:

```json
Condition translator output:
[
  {
    "signature": "isOpen()",
    "name": "isOpen",
    "containingClass": {
      "qualifiedName": "net.Connection",
      "name": "Connection",
      "isArray": false
    },
    "targetClass": "net.Connection",
    "isVarArgs": false,
    "returnType": {
      "qualifiedName": "boolean",
      "name": "boolean",
      "isArray": false
    },
    "parameters": [],
    "paramTags": [],
    "throwsTags": []
  },
  {
    "signature": "open()",
    "name": "open",
    "containingClass": {
      "qualifiedName": "net.Connection",
      "name": "Connection",
      "isArray": false
    },
    "targetClass": "net.Connection",
    "isVarArgs": false,
    "returnType": {
      "qualifiedName": "void",
      "name": "void",
      "isArray": false
    },
    "parameters": [],
    "paramTags": [],
    "throwsTags": [
      {
        "exceptionType": {
          "qualifiedName": "java.lang.IllegalStateException",
          "name": "IllegalStateException",
          "isArray": false
        },
        "codeTags": [],
        "comment": "the connection is already open.",
        "kind": "THROWS",
        "condition": "receiverObjectID.isOpen()"
      }
    ]
  },
  {
    "signature": "send(java.lang.String message)",
    "name": "send",
    "containingClass": {
      "qualifiedName": "net.Connection",
      "name": "Connection",
      "isArray": false
    },
    "targetClass": "net.Connection",
    "isVarArgs": false,
    "returnType": {
      "qualifiedName": "void",
      "name": "void",
      "isArray": false
    },
    "parameters": [
      {
        "type": {
          "qualifiedName": "java.lang.String",
          "name": "String",
          "isArray": false
        },
        "name": "message"
      }
    ],
    "paramTags": [],
    "throwsTags": [
      {
        "exceptionType": {
          "qualifiedName": "java.lang.NullPointerException",
          "name": "NullPointerException",
          "isArray": false
        },
        "codeTags": [],
        "comment": "message is null.",
        "kind": "THROWS",
        "condition": "args[0]==null"
      }
    ]
  }
]
```

New directory structure after Toradocu run:

```
tutorial/
├── aspects
│   ├── aop.xml
│   ├── Aspect_1.java
│   ├── Aspect_2.java
│   └── TestCaseAspect.java
├── lib
│   ├── hamcrest-core-1.3.jar
│   └── junit-4.12.jar
├── README.md
├── src
│   └── net
│       ├── Connection.class
│       └── Connection.java
└── test
    └── net
        ├── ConnectionTest.class
        └── ConnectionTest.java

7 directories, 11 files
```

## Compile the generated aspects and weave them into the test suite of the system under test:

Compiling

```shell
javac -g -cp lib/aspectjrt-1.8.9.jar:src:lib/junit-4.12.jar aspects/*.java
```

Weaving

```shell
java -cp lib/aspectjtools-1.8.9.jar:lib/aspectjweaver-1.8.9.jar:lib/aspectjrt-1.8.9.jar:lib/junit-4.12.jar:src org.aspectj.tools.ajc.Main -inpath aspects:test -outjar weaved_testsuite.jar -showWeaveInfo -source 1.8 -target 1.8
```

Directory structure after waving process:

```
tutorial/
├── aspects
│   ├── aop.xml
│   ├── Aspect_1.class
│   ├── Aspect_1.java
│   ├── Aspect_2.class
│   ├── Aspect_2.java
│   ├── TestCaseAspect$ExpectedException.class
│   ├── TestCaseAspect$InvalidParamException.class
│   ├── TestCaseAspect.class
│   └── TestCaseAspect.java
├── lib
│   ├── aspectjrt-1.8.9.jar
│   ├── aspectjtools-1.8.9.jar
│   ├── aspectjweaver-1.8.9.jar
│   ├── hamcrest-core-1.3.jar
│   └── junit-4.12.jar
├── README.md
├── src
│   └── net
│       ├── Connection.class
│       └── Connection.java
├── test
│   └── net
│       ├── ConnectionTest.class
│       └── ConnectionTest.java
└── weaved_testsuite.jar

7 directories, 20 files
```

## Run the test suite augmented with Toradocu's oracles:

```shell
java -cp lib/junit-4.12.jar:lib/hamcrest-core-1.3.jar:src:weaved_testsuite.jar:lib/aspectjrt-1.8.9.jar org.junit.runner.JUnitCore net.ConnectionTest
```

Test output:

```
JUnit version 4.12
.E.Triggered aspect: Aspect_2 (ConnectionTest.java:20) -> Success: Expected exception caught

Time: 0,008
There was 1 failure:
1) open(net.ConnectionTest)
java.lang.AssertionError: Triggered aspect: Aspect_1 (ConnectionTest.java:13) -> Failure: Expected exception not thrown. Expected exceptions were: java.lang.IllegalStateException 
	at org.junit.Assert.fail(Assert.java:88)
	at Aspect_1.advice(Aspect_1.java:36)
	at net.ConnectionTest.open_aroundBody4(ConnectionTest.java:13)
	at net.ConnectionTest.open_aroundBody5$advice(ConnectionTest.java:11)
	at net.ConnectionTest.open(ConnectionTest.java:1)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:498)
	at org.junit.runners.model.FrameworkMethod$1.runReflectiveCall(FrameworkMethod.java:50)
	at org.junit.internal.runners.model.ReflectiveCallable.run(ReflectiveCallable.java:12)
	at org.junit.runners.model.FrameworkMethod.invokeExplosively(FrameworkMethod.java:47)
	at org.junit.internal.runners.statements.InvokeMethod.evaluate(InvokeMethod.java:17)
	at org.junit.runners.ParentRunner.runLeaf(ParentRunner.java:325)
	at org.junit.runners.BlockJUnit4ClassRunner.runChild(BlockJUnit4ClassRunner.java:78)
	at org.junit.runners.BlockJUnit4ClassRunner.runChild(BlockJUnit4ClassRunner.java:57)
	at org.junit.runners.ParentRunner$3.run(ParentRunner.java:290)
	at org.junit.runners.ParentRunner$1.schedule(ParentRunner.java:71)
	at org.junit.runners.ParentRunner.runChildren(ParentRunner.java:288)
	at org.junit.runners.ParentRunner.access$000(ParentRunner.java:58)
	at org.junit.runners.ParentRunner$2.evaluate(ParentRunner.java:268)
	at org.junit.runners.ParentRunner.run(ParentRunner.java:363)
	at org.junit.runners.Suite.runChild(Suite.java:128)
	at org.junit.runners.Suite.runChild(Suite.java:27)
	at org.junit.runners.ParentRunner$3.run(ParentRunner.java:290)
	at org.junit.runners.ParentRunner$1.schedule(ParentRunner.java:71)
	at org.junit.runners.ParentRunner.runChildren(ParentRunner.java:288)
	at org.junit.runners.ParentRunner.access$000(ParentRunner.java:58)
	at org.junit.runners.ParentRunner$2.evaluate(ParentRunner.java:268)
	at org.junit.runners.ParentRunner.run(ParentRunner.java:363)
	at org.junit.runner.JUnitCore.run(JUnitCore.java:137)
	at org.junit.runner.JUnitCore.run(JUnitCore.java:115)
	at org.junit.runner.JUnitCore.runMain(JUnitCore.java:77)
	at org.junit.runner.JUnitCore.main(JUnitCore.java:36)

FAILURES!!!
Tests run: 2,  Failures: 1
```

All steps are accordantly the tutorial.