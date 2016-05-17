# Example usage of sbt-scalafmt plugin.

* Run `sbt scalafmt` to format `Foobar.scala`.
* Run `sbt scalafmtTest` to throw an exception because `Foobar.scala` is
  mis-formatted.
* If you have a multi-project build and the custom `.scalafmt` configuration is
  not picked up, make sure that `scalafmtConfig := Some(file(.scalafmt))` for
  all of your projects and not only the root project.
  **Tip.** Use `show scalafmtConfig` to verify this.

