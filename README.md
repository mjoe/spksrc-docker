Dockerfile for image mjoe/spksrc

automated build
``
archs=`cd /spksrc/toolchains && ls -d *-5.2 && cd -`
make `for d in $archs; do echo ${d}|sed 's/syno/arch/g' ;done | xargs`
``
