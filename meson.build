project(
    'alpine-make-oci', 
    license : 'MIT',
    version: '0.1.0'
)

find_program('buildah')
find_program('alpine-make-rootfs')

prefix = get_option('prefix')

configure_file(
    input: 'alpine-make-oci',
    output: 'alpine-make-oci',
    install: true,
    install_dir : join_paths(prefix,'bin'),
    install_mode: 'rwxr-xr-x',
    copy: true
)
