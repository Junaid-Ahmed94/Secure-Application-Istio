## Milestone 2

**Question** Explanation of whether the request is proxied by the ingress gateway to the frontend service or not based on the access log message.   
**Answer** As per the Access log, all the upstream addresses are pointing to local host or local service `"upstream_local_address": "127.0.0.1:41664"`, `"upstream_host": "127.0.0.1:8080"`, `"upstream_cluster": "inbound|80|http|frontend-external.online-boutique.svc.cluster.local"`. So it seems so that all request was proxied.

