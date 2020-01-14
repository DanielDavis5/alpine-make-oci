project('alpine-make-oci')

prefix = get_option('prefix')

find_program('alpine-make-rootfs')

configure_file(
    input: 'alpine-make-oci',
    output: 'alpine-make-oci',
    install: true,
    install_dir : join_paths(prefix,'bin'),
    install_mode: 'rwxr-xr-x',
    copy: true
)
