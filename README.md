# Libling Skeleton

Just a minimal example of how a libling is structured.

## Try it

Add this libling to your sbt project:

* `project/plugins.sbt`
    
      resolvers += Resolver.bintrayIvyRepo("jastice","sbt-plugins")    
      addSbtPlugin("libling" % "sbt-hackling" % "0.1+32-375617a1")

* `build.sbt`

      sourceDependencies += Dependency(
        Version("20b4f2e74257988de6d49e17fc2fda622d48badc"),
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