## Welcome to Data Developer and Engineer Organization 👋

For document of this organization, you can follow this like [Document](http://ddeutils.github.io/ddedocs).

## Organization Components

This organization has the propose to make lightweight data orchestration framework for small to
middle project scale (1-1000 workflows).

Firstly, I will implement base projects, [Core](https://github.com/ddeutils/ddeutil) and [IO](https://github.com/ddeutils/ddeutil-io)
for the first dependency packages because it has a lot of base code to make main package and I do
not want to develop this code on the main package, for example, it do not good if I want fix bug
on the merge key function that no relate with the workflow package

The main package of my orchestration framework has 2 layer and I split it to 2 projects for
optional installation when you want to only use just one of these layers.

- [Workflow](https://github.com/ddeutils/ddeutil-workflow) - executor pipeline on a worker node.
- [Observe](https://github.com/ddeutils/ddeutil-observe) - web application for observe logging on a server node.

> [!NOTE]
> I have some 3rd-party projects for keeping an additional practices to use any 3rd API connect
> data source, like `polars`, `duckdb`, etc.
> - [Vendors](https://github.com/ddeutils/ddeutil-vendors)
