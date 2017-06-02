# Libling Skeleton

Just a minimal example of how a libling is structured.

## Try it

Add this libling to your sbt project:

* `project/plugins.sbt`
    
      resolvers += Resolver.bintrayIvyRepo("jastice","sbt-plugins")    
      addSbtPlugin("libling" % "sbt-hackling" % "0.2.1")

* `build.sbt`

      sourceDependencies += Dependency(
        Version("ef33ab5a6eac7af6b2f6a8d238ccdc88e25171a2"),
        Repositories(uri("https://github.com/libling/libling-skeleton.git")))

I promise this will become easier and prettier.

On the sbt shell:

    > liblingUpdate
    > liblingInstall
    
Yes, currently updating and installing are separate steps. How inconvenient!

In your code:

```scala
object main extends App {
  println(cellar.skeleton.fish)
}
```