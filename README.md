# Composite actions for Halo

1. Docker build for Halo

   ```yaml
   uses: halo-sigs/actions/halo-next-docker-build@main # prefer to specific ref.
   with:
     ghcr_token: ${{ secrets.GHCR_TOKEN }} # default is ""
     push: true # default is false
     image-name: halodev # default is halo
     checkout-from: next # default is default branch
   ```
