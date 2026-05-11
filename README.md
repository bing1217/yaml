# yaml
```
[root@localhost bin]# ./istioctl proxy-config routes deploy/istio-ingressgateway -n istio-system
NAME                                                    VHOST NAME                       DOMAINS                       MATCH                  VIRTUAL SERVICE
http.8080                                               *:80                             *                             /*                     bookinfo.default
http.8080                                               grafana.liubingjie.com:80        grafana.liubingjie.com        /*                     grafana-virtualservice.istio-system
http.8080                                               jaeger.liubingjie.com:80         jaeger.liubingjie.com         /*                     jaeger.istio-system
http.8080                                               kiali.liubingjie.com:80          kiali.liubingjie.com          /*                     kiali-virtualservice.istio-system
http.8080                                               loki.liubingjie.com:80           loki.liubingjie.com           /*                     loki.istio-system
http.8080                                               prometheus.liubingjie.com:80     prometheus.liubingjie.com     /*                     prometheus-virtualservice.istio-system
http.8080                                               skywalking.liubingjie.com:80     skywalking.liubingjie.com     /*                     skywalking-virtualservice.istio-system
http.8080                                               tracing.liubingjie.com:80        tracing.liubingjie.com        /*                     tracing-virtualservice.istio-system
https.443.https.argocd-gateway.argocd                   argocd.liubingjie.com:443        argocd.liubingjie.com         /*                     argocd-vs.argocd
https.443.https.argo-rollouts-gateway.argo-rollouts     rollout.liubingjie.com:443       rollout.liubingjie.com        /*                     argo-rollouts-vs.argo-rollouts
                                                        backend                          *                             /healthz/ready*
                                                        backend                          *                             /stats/prometheus*
=======
                                                        backend                          *                             /healthz/ready*        
                                                        backend                          *                             /stats/prometheus*     
```
