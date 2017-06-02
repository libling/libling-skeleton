# Libling Skeleton

Just a minimal example of how a libling is structured.

## Try it

Add this libling to your sbt project:

* `project/plugins.sbt`
    
      resolvers += Resolver.bintrayIvyRepo("jastice","sbt-plugins")    
      addSbtPlugin("libling" % "sbt-hackling" % "0.1+32-375617a1")

* `build.sbt`

      sourceDependencies += Dependency(
        Version("165047f978851daf46c94e4cef3456b684dab23e"),
        Repositories(uri("https://github.com/libling/libling-skeleton.git")))

I promise this will become easier and prettier.

On the sbt shell:

    > liblingUpdate
    > liblingInstall
    
Yes, currently updating and installing are separate steps. How inconvenient!

In your code:

```scala
object main extends App {
  println(skeleton.fish)
}
```