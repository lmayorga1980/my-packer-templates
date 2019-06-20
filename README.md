## My Packer Templates

Builds serveral Packer Templates(AWS, Vagrant or anything interesting)

## Requirements

* Packer `1.3.x`.
* VirtualBox `6.x` - VirtualBox Download https://www.virtualbox.org/wiki/Downloads
* Amazon Access Keys configured in `$HOME/.aws/credentials` - http://docs.aws.amazon.com/cli/latest/userguide/cli-chap-getting-started.html
* Configure your environment variables - For OSX `~./bashrc` with the "AWS_S3_BUCKET" or Windows System Variables.

## How does it work

* Validate a Packer template `packer validate <template_name>.json`.
* Run a Packer build `packer build <template_name>.json`.
* Run a Packer build with variables `packer -var-file myvariables.json <template_name>.json`

## References

* Packer Amazon Import Post-Processor - https://www.packer.io/docs/post-processors/amazon-import.html
* Amazon Import Process - http://docs.aws.amazon.com/vm-import/latest/userguide/vmimport-image-import.html
* Packer VMware ESXI - https://www.packer.io/docs/builders/vmware-iso.html
