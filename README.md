## Nuxeo ECM custom runtime template used by the Indianapolis Museum of Art

The custom runtime template for the Nuxeo ECM (http://www.nuxeo.com) used by the Indianapolis Museum of Art. It is used in production by the IMA and provided publicly for the reference of others.

This code is made available under the same LGPL license as Nuxeo. See LICENSE.txt for details.

### Deploying

This repository should be installed at `%nuxeo%/templates/ima`. It is important to rename the top-level folder from `ima-nuxeo-template` to `ima` for the deployment to work correctly.

All variables seen (ex. `${variable.name}`) should be declared in the `%nuxeo/bin/nuxeo.conf` file before starting the nuxeo server. Additionally, `ima` should be added to the `nuxeo.templates` variable. For example, our installation has `nuxeo.templates=postgresql,ima,dam`.
