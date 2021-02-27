```
istioctl proxy-config endpoints $INGRESS_POD.istio-system --cluster 'outbound|80||frontend.online-boutique.svc.cluster.local' -o json
[
    {
        "name": "outbound|80||frontend.online-boutique.svc.cluster.local",
        "addedViaApi": true,
        "hostStatuses": [
            {
                "address": {
                    "socketAddress": {
                        "address": "10.60.1.6",
                        "portValue": 8080
                    }
                },
                "stats": [
                    {
                        "name": "cx_connect_fail"
                    },
                    {
                        "value": "4",
                        "name": "cx_total"
                    },
                    {
                        "name": "rq_error"
                    },
                    {
                        "value": "22",
                        "name": "rq_success"
                    },
                    {
                        "name": "rq_timeout"
                    },
                    {
                        "value": "22",
                        "name": "rq_total"
                    },
                    {
                        "type": "GAUGE",
                        "value": "4",                        
                        "name": "cx_active"
                    },
                    {
                        "type": "GAUGE",
                        "name": "rq_active"
                    }
                ],
                "healthStatus": {
                    "edsHealthStatus": "HEALTHY"
                },
                "weight": 1,
                "locality": {
                    "region": "us-central1",
                    "zone": "us-central1-c"
                }
            },
            {
                "address": {
                    "socketAddress": {
                        "address": "10.60.4.15",
                        "portValue": 8080
                    }
                },
                "stats": [
                    {
                        "name": "cx_connect_fail"
                    },
                    {
                        "name": "cx_total"
                    },
                    {
                        "name": "rq_error"
                    },
                    {
                        "name": "rq_success"
                    },
                    {
                        "name": "rq_timeout"
                    },
                    {
                        "name": "rq_total"
                    },
                    {
                        "type": "GAUGE",
                        "name": "cx_active"
                    },
                    {
                        "type": "GAUGE",
                        "name": "rq_active"
                    }
                ],
                "healthStatus": {
                    "edsHealthStatus": "HEALTHY"
                },
                "weight": 1,
                "locality": {
                    "region": "us-central1",
                    "zone": "us-central1-c"
                }
            }
        ]
    }
]
```