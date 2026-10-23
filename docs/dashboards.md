# Dashboards

One dashboard per service, provisioned from `grafana/provisioning/dashboards/`. Each carries the tag of its service, which
is how the portal finds it (`grafana/dashboard-selector: tags @> '<tag>'`).

!!! note "Links"
    The links point at `https://grafana.platform-demo.click`. Grafana is not deployed on the EKS cluster at the moment, so they do not
    resolve until it is; in the docker compose stack the same dashboards are at <http://localhost:3000>.

| Dashboard | uid | Link |
|---|---|---|
| Ad Service | `ad-service-overview` | [open](https://grafana.platform-demo.click/d/ad-service-overview) |
| Cart Service | `cart-service-overview` | [open](https://grafana.platform-demo.click/d/cart-service-overview) |
| Checkout Service | `checkout-service-overview` | [open](https://grafana.platform-demo.click/d/checkout-service-overview) |
| Currency Service | `currency-service-overview` | [open](https://grafana.platform-demo.click/d/currency-service-overview) |
| Email Service | `email-service-overview` | [open](https://grafana.platform-demo.click/d/email-service-overview) |
| Frontend Service | `frontend-overview` | [open](https://grafana.platform-demo.click/d/frontend-overview) |
| Payment Service | `payment-service-overview` | [open](https://grafana.platform-demo.click/d/payment-service-overview) |
| Product Catalog Service | `product-catalog-overview` | [open](https://grafana.platform-demo.click/d/product-catalog-overview) |
| Recommendation Service | `recommendation-service-overview` | [open](https://grafana.platform-demo.click/d/recommendation-service-overview) |
| Shipping Service | `shipping-service-overview` | [open](https://grafana.platform-demo.click/d/shipping-service-overview) |

All 198 dashboard queries were run against a live stack; 186 return data and the remaining 12 are error-rate and
status-code panels that are empty simply because nothing failed.
