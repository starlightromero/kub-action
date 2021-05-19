# Kubernetes Practice

## Notes

Kubernetes will only pull images with new tags. It is best to use versioning for your containers

## Commands

`kubectl set image deployment/DEPLOYMENT_NAME CONTAINER_NAME=IMAGE_NAME` = update deployment

`kubectl rollout status deployment/DEPLOYMENT_NAME` = inspect rollout progress

`kubectl rollout undo deployment/DEPLOYMENT_NAME` = rollback deployment

`kubectl rollout history deployment/DEPLOYMENT_NAME` = see deployment history

`kubectl rollout history deployment/DEPLOYMENT_NAME --revision=REVISION_ID` = get details for a specific deployment revision

`kubctl rollout undo deployment/DEPLOYMENT_NAME --to-revision=REVISION_ID` = rollback deployment to a specific revision

`kubectl delete deployments,services -l KEY=VALUE` = delete deployments and services by label
