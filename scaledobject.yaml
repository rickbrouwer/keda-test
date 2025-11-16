apiVersion: keda.sh/v1alpha1
kind: ScaledObject
metadata:
  name: worker-scale
spec:
  scaleTargetRef:
    name: worker
  minReplicaCount: 1
  maxReplicaCount: 3
  triggers:
  - type: cron
    metadata:
      timezone: Europe/Amsterdam
      start: 0 6 * * *
      end: 0 23 * * *
      desiredReplicas: "2"

