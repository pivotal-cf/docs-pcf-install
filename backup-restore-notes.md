for stopping and starting cc vms, they don't start with "api". they start with "cloud_controller_" but not the "cloud_controller-worker" ones. (that won't hurt, but unnecessary)

NSF server, not "the" Nfs...

for this: Stop Cloud Controller by running bosh -d DEPLOYMENT-MANIFEST stop SELECTED-VM for each Cloud Controller VM. Example:

-d flag and manifest are optional (needed if multiple deployments)

