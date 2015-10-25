This code example shows how to setup sbt to use a customized Slick code-generator for working with an existing database schema. `project/Build.scala` enables automatically as well as manually triggered code-generation. `codegen/CustomizedCodeGenerator.scala` contains the code customizing Slick's code-generator. `codegen/Config.scala` contains some shared configuration code between the code-generator and the main project. `src/main/scala/Example.scala` uses the generated code. The code is generated into file `target/scala-2.11/src_managed/slick/demo/Tables.scala`. The location can be changed in the sbt script. It is usally wise to keep the generated Slick code under version control.
