# GitOps & Flux Demo

## Part 1

-   show how flux is running in the cluster `kubectl get deployments -n flux-system`
-   take a look at the logs `kubectl logs flux{tab} -n flux-system`

## Part 2

-   take a look a example app `kubectl get deployments -n example-app`
-   change the deployment through the state repository
-   introduction fluxctl (`fluxctl sync --k8s-fwd-ns flux-system`)
-   verify that change was successful
-   delete contents of state repository and verify

## Part 3

-   commit setup with dev and staging environment
-   apply new setup through state-repository
-   showcase what happens when accidental kubectl apply is excecuted

## Part 4

-   add prod environment & show setup of second flux
-   push to cluster-A
-   verify that nothing changed
-   merge request to prod branch
-   show changes to prod
-   do another release to prod
-   rollback

## part 5

-   Showcase multi-tenancy setup (https://github.com/fluxcd/multi-tenancy)
