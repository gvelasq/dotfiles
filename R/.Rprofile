if (interactive()) {
  suppressMessages(require(devtools))
  suppressMessages(require(usethis))
}
if (Sys.info()[["sysname"]] == "Linux") {
  options(
    # https://packagemanager.rstudio.com/__docs__/admin/serving-binaries/#binary-user-agents
    HTTPUserAgent = sprintf("R/%s R (%s)", getRversion(), paste(getRversion(), R.version["platform"], R.version["arch"], R.version["os"])),
    repos = c(
      gvelasq = "https://gvelasq.r-universe.dev",
      REPO_NAME = "https://packagemanager.rstudio.com/all/__linux__/jammy/latest"
    )
  )
}
options(
  usethis.description = list(
    `Authors@R` = 'person("First", "Last", email = "", role = c("aut", "cre"))',
    License = "MIT + file LICENSE",
    Version = "0.0.0.9000"
  ),
  usethis.full_name = "First Last",
  usethis.protocol = "https",
  vsc.rstudioapi = TRUE,
  warnPartialMatchArgs = TRUE,
  warnPartialMatchDollar = TRUE,
  warnPartialMatchAttr = TRUE
)
