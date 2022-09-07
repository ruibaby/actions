# Composite actions for Halo

1. Docker build for Halo

   ```yaml
   uses: halo-sigs/actions/halo-next-docker-build@main # prefer to specific ref.
   with:
     ghcr_token: ${{ secrets.GHCR_TOKEN }} # default is ""
     dockerhub-user: halohub
     dockerhub-token: ${{ secrets.DOCKERHUB_TOKEN }}
     push: true # default is false
     image-name: halodev # default is halo
     checkout-from: next # default is default branch
   ```

1. Docker build for Halo admin

   ```yaml
   uses: halo-sigs/actions/admin-next-docker-build-push@main # prefer to specific ref.
   with:
     ghcr_token: ${{ secrets.GHCR_TOKEN }} # default is ""
     dockerhub-user: halohub
     dockerhub-token: ${{ secrets.DOCKERHUB_TOKEN }}
     push: true # default is false
     image-name: halodev # default is halo
     checkout-from: next # default is default branch
   ```
