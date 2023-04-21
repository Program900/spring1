# spring1
multi-module Maven project and manage dependencies across modules.
A multi-module Maven project is a project that consists of multiple modules, 
each with its own pom.xml file and source code.
The modules are then grouped together into a parent project that manages their dependencies
and builds them in the correct order.

the benefits of a multi-module project and when it makes sense to use one
 the process of creating a multi-module project
including creating the parent project and adding child modules.
 how to manage dependencies between modules using the dependencyManagement 
section in the parent pom.xml file.
Why Multi-Module Project?
The major benefits of making multi-module projects are

One single command is required to build all projects, including the submodules.
Maven always cares about the build order for you. You don't need to worry about that.
In most cases, the sub-modules depend on other modules.
So the build order matters while building the project.
Multimodule project configuration on your CI server is so easy.
One single job can handle everything.
Can build and work with a single module itself. 
Suppose in your multi-module project there are different teams are working
on different modules. You don't need to worry about others' work,
and you can work by importing your own submodule.
parent pom
The main difference between multi-module parent pom and normal pom is its packaging type. 
For a multi-module parent pom, its packaging type becomes ‘pom’.
