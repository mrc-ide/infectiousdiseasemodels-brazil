local({
  use_bundled_lib <- function() {
    lib_filename <- "lib-2019"
    root <- normalizePath("/", mustWork = TRUE)
    f <- function(path) {
      if (file.exists(file.path(path, lib_filename))) {
        return(path)
      }
      if (normalizePath(path, mustWork = TRUE) == root) {
        return(NULL)
      }
      Recall(file.path("..", path))
    }
    path <- f(".")
    if (is.null(path)) {
      warning("Hit the root without finding bundled library",
              immediate. = TRUE)
      return()
    }
    path <- normalizePath(file.path(path, lib_filename), mustWork = TRUE)
    message(sprintf("Using library at '%s'", path))
    .libPaths(path)
  }
  use_bundled_lib()
})
