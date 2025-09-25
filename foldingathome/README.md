## Folding@home
A program donating computing resources to science by simulating protein folding.

There is a `foldingathome` volume that you do need to keep in mind.

For ideal results, make sure your virtual machine has access to a GPU (preferably NVIDIA).

When deploying in Portainer, make sure to add a `stack.env` file for secrets with this variable set:
- `ACCOUNT_TOKEN` - Folding@home login token