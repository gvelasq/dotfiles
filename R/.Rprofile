if (interactive()) {
  suppressMessages(require(devtools))
  suppressMessages(require(usethis))
}
if (Sys.info()[["sysname"]] == "Linux") {
  options(
    # https://packagemanager.posit.co/__docs__/admin/serving-binaries/#binary-user-agents
    HTTPUserAgent = sprintf("R/%s R (%s)", getRversion(), paste(getRversion(), R.version["platform"], R.version["arch"], R.version["os"])),
    repos = c(
      gvelasq = "https://gvelasq.r-universe.dev",
      REPO_NAME = "https://packagemanager.posit.co/cran/__linux__/jammy/latest"
    )
  )
}
options(
  usethis.description = list(
    `Authors@R` = 'person("First", "Last", email = "", role = c("aut", "cre"))',
    License = "MIT + file LICENSE",
    Version = "0.0.0.9000"
  ),
  usethis.destdir = "~/rrr",
  usethis.full_name = "First Last",
  usethis.protocol = "https",
  warnPartialMatchArgs = TRUE,
  warnPartialMatchDollar = TRUE,
  warnPartialMatchAttr = TRUE
)
.domain <- "github.com" # replace with target domain
.remotes <- tryCatch(usethis::git_remotes(), error = function(e) NULL)
if (!is.null(.remotes) && grepl(.domain, .remotes$origin)) {
  usethis::use_git_config(scope = "project", user.email = "author@noreply.github.com") # replace with target email
  cli::cli_alert_success("{ .domain } remote detected and local git options applied")
}
rm(.domain, .remotes)
