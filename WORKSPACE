workspace(name = 'torrent')

load('//bazel:workspace.bzl', torrent_repositories = 'repositories')
torrent_repositories()

load('@io_bazel_rules_pex//pex:pex_rules.bzl', 'pex_repositories')
pex_repositories()

load('@io_bazel_rules_docker//container:container.bzl',
    container_repositories = 'repositories',
)
container_repositories()
load('@io_bazel_rules_docker//cc:image.bzl',
    _cc_image_repos = 'repositories',
)
_cc_image_repos()
