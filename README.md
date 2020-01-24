# rhunter.org source

This is the [Hugo](https://gohugo.io/) source for [rhunter.org](https://rhunter.org), currently using the [Notepadium](https://themes.gohugo.io/hugo-notepadium/) theme.

I use [`SSH` and `rsync`](https://gohugo.io/hosting-and-deployment/deployment-with-rsync/) to deploy the site to [NFSN](https://www.nearlyfreespeech.net/) using the following `bash` script:

    #!/bin/sh

    USER= # my username
    HOST=ssh.phx.nearlyfreespeech.net
    DIR=/home/public/

    rsync -avz --delete public/ ${USER}@${HOST}:/${DIR} --exclude=/.well-known

    exit 0

The `--exclude` option prevents my [Let's Encrypt](https://letsencrypt.org/) directory (`.well-known`) from being deleted every time I deploy.
